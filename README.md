# JustWantToSee.github.io

个人简历站点（Jekyll + [resume-theme](https://github.com/sproogen/resume-theme)）。

## 编辑内容

主要配置在 `_config.yml`：`about_*` 为自我介绍，`content` 为各区块（Projects / Experience / Education 等）。

### 常见坑：同一段里不要写两个 `content:`

在 YAML 里，**同一个缩进层级如果出现两次相同的键名**（例如两个 `content:`），解析时通常会**只保留最后一个**，前面的条目会被悄悄丢掉。所以「工作经历」「教育背景」里有多条时，应写在**同一个** `content:` 下面，用列表 `-` 列出多条，而不是再写第二个 `content:`。

部署推送后若页面未更新，可等待 GitHub Pages 构建完成或强制刷新浏览器缓存。