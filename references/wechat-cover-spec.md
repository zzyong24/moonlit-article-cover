# 公众号封面规格与出处（核实于 2026-10-21，北京时间）

| 项 | 结论 | 可信度 | 出处 |
|---|---|---|---|
| 图文消息封面只有两种裁切比例：**2.35:1** 和 **1:1** | 草稿接口 `cover_info.crop_percent_list` 的 `ratio` 仅支持 `2.35_1`、`1_1`（图文消息 news） | **官方开发文档** | https://developers.weixin.qq.com/doc/subscription/api/draftbox/draftmanage/api_draft_update |
| 两种裁切出自同一张原图，坐标以原图左上 (0,0)、右下 (1,1) 计；编辑器 JSAPI 不填坐标默认居中裁 | `picCrop_235_1`、`picCrop_1_1` | **官方开发文档** | https://developers.weixin.qq.com/doc/subscription/guide/product/mp_editor_jsapi.html |
| 星标、常读用户在订阅号消息列表看到 2.35:1 大图；其他用户看到 1:1 小图 | 开放社区答复 | 社区答复，答复者身份未核实，未见正式文档 | https://developers.weixin.qq.com/community/develop/doc/000ae49c710848c6967d06b3d52800 |
| 头条最佳 900×383 px，次条 1:1 最佳 383×383 px | 开放社区答复（2023-08-09） | 同上，未见正式文档 | https://developers.weixin.qq.com/community/develop/doc/000ca6640208a083702030c9e61000 |

注意：有的第三方资料把 900×383 写成「3:1」，这是错的，900÷383≈2.35。

## 本 skill 的交付口径（团队自定）

- **主图 1880×800 PNG**（正好 2.35:1，宽度约为 900 的 2 倍，留高清余量）。
- **1:1 框**：默认 x 40–840、y 0–800（比例坐标 x1 0.0213、y1 0、x2 0.4468、y2 1）。主标题，至少重点词，必须完整落在框内。框位写进 manifest，发布环节按它填裁切坐标；不填就会被居中裁，标题可能被切。
- **安全区**：四边 ≥ 60 px。官方没写遮挡位置，首次进草稿后在手机消息列表里截图核对两种裁切。
- 同题 X 版可居中裁掉左右各 60 px 得到公众号主图；主标题放不进 1:1 框时单独出公众号版。
- 封面不用作者真人照片或真人 IP，与公众号发布环节的规则一致。
