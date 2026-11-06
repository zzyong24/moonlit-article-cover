# 月明·文章封面

为 X（推特）长文 Articles 和微信公众号文章制作锚点式横幅封面：一个承诺、一个主锚点、一个重点词、一个钩子胶囊，配一个与命题相关的示意物。

## 你会得到什么

- X 长文 5:2（2000×800）封面
- 公众号 2.35:1 主封面，并标好 1:1 转发裁切框
- 封面方案五件套、提示词、安全区检查与 manifest

## 试着这样说

```text
用 moonlit-article-cover。给这篇文章做一张 X 长文 5:2 封面和一张公众号封面，先写五件套方案，按题材配色，不用人像。
```

## 安装与首次使用

将本仓库的完整目录交给支持本地 Skill 的 Agent 安装，保留 `SKILL.md` 与随附资源。已有同名版本时先检查差异；使用版本锁的工作区沿用自身升级机制。

让 Agent 安装：

```text
请安装这个 Skill：https://github.com/zzyong24/moonlit-article-cover
```

也可通过 Skills CLI 安装：

```bash
npx skills add zzyong24/moonlit-article-cover
```

## 配置与依赖

需要文章标题或定稿正文、一句话主判断、1–3 个可核对要点和目标平台。默认使用 image_gen / gpt-image 类图像生成工具出 PNG；HTML/SVG 只用于排字预览，不冒充封面。

## 数据与使用边界

文案与提示词会交给图像生成服务。文章封面默认不用人像；只有选题没有正文时只能做方向稿。本 Skill 不上传、不发布，成图需作者逐条确认后才交给发布环节。

## 配套 Skill

[video-cover](https://github.com/zzyong24/moonlit-video-cover) · [wechat-article](https://github.com/zzyong24/moonlit-wechat-article) · [wechat-publisher](https://github.com/zzyong24/moonlit-wechat-publisher) · [social-publisher](https://github.com/zzyong24/moonlit-social-publisher)

## 详细说明

执行流程与资源导航见 [SKILL.md](SKILL.md)。安装检查不代表真实业务验收；需要外部服务、账号登录或付费生成的步骤，应在使用者自己的环境中验证。

---

月明水清深 · `moonlit-article-cover`
