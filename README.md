# 留白 · 言情写作

中文言情小说写作 Skill 与静态网页落地页。以约五千字短篇为目标，通过人物对立、物件叙情、生活化对白和含蓄结尾，构建有起伏的感情故事。

## 内容

- `skills/romance-fiction/`：可安装的 Codex Skill，按开篇、中段、结尾组织写作要求，附修改示例。
- `website/`：最终网页源码，含响应式布局、叙情示例切换、提示词生成与复制、Skill 下载。
- `offline/留白-离线版.html`：可直接用浏览器打开的单文件离线版。

## 安装 Skill

将 `skills/romance-fiction` 目录复制到 `~/.codex/skills/`。在 Codex 中使用：

```text
请用 $romance-fiction 写一篇五千字左右的中文言情小说。
```

Skill 默认强调虐恋基调、首句悬念、集中冲突、伏笔回收、口语化且有区分度的对白，以及以具体动作、物件和环境承载情绪。小说正文不采用编号分章，每段首行空两个汉字，标题居中。

## 预览网页

网页使用原生 HTML、CSS 和 JavaScript，无需安装依赖。

```sh
python3 -m http.server 8000 --directory website
```

访问 http://localhost:8000 。也可直接打开离线 HTML。网页生成写作提示词，实际小说创作需在支持 Skill 的助手中完成。

## 发布静态网站

可将 `website/` 目录部署到 GitHub Pages 或其他静态托管服务。请将这一路径设为站点根目录，保留 `assets/` 下载资源。

## 开源许可

Skill、网页源码与项目附带素材使用 [MIT License](LICENSE)，可使用、修改和再分发，须保留版权及许可声明。
