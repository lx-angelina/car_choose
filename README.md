# 40 万落地 · 纯电 SUV 选购结论（2026.11）

一份单文件静态报告。`index.html` 已内联全部样式，无外部依赖、无网络请求、无跟踪脚本，拷走一个文件即可打开。

## 文件说明

| 文件 | 用途 |
| --- | --- |
| `index.html` | 报告本体，GitHub Pages 的默认入口 |
| `README.md` | 本说明，不会被渲染成网页 |

## 方式一：GitHub Pages（生成公开链接）

1. 在 GitHub 新建一个仓库，例如 `suv-report`，可见性选 **Public**。
2. 把 `index.html` 和 `README.md` 上传到仓库根目录。
3. 打开仓库的 **Settings → Pages**。
4. **Source** 选 `Deploy from a branch`，**Branch** 选 `main`，目录选 `/ (root)`，点 Save。
5. 等 1 分钟左右，访问 `https://<你的用户名>.github.io/suv-report/`。

## 方式二：命令行上传

```bash
git init
git add index.html README.md
git commit -m "add SUV comparison report"
git branch -M main
git remote add origin https://github.com/<用户名>/<仓库名>.git
git push -u origin main
```

推送完成后按上面的步骤 3–5 开启 Pages。

## 注意事项

- 免费账户的 GitHub Pages 只对 **Public** 仓库开放；Private 仓库需要 GitHub Pro 及以上。
- 仓库名会直接成为路径的一部分，建议用小写英文，例如 `suv-report`。
- 需要自定义域名时，在 **Settings → Pages → Custom domain** 中配置，并按提示添加 CNAME 记录。
- 报告为静态页面，更新内容只需替换 `index.html` 后重新提交，Pages 会在一分钟内自动刷新。
