蓝图官网官网【Q-——333307——】蓝图官网官网【 辋芷《888yx●vip》 】
蓝图官网官网【Q-——333307——】蓝图官网官网【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程（2025版）

还在羡慕别人拥有独立博客？其实通过 GitHub Pages 和 Hexo，你可以在半小时内拥有一个免费、高速、可自定义的专属技术博客。今天手把手教你从环境配置到发布上线，全程图文详解。

 为什么选择 GitHub Pages + Hexo？

- 完全免费：托管在 GitHub 服务器，无需购买云主机
- CDN 加速：国内访问速度快，适合技术内容分享
- SEO 友好：生成静态 HTML，搜索引擎收录率高
- 版本管理：文章和代码都纳入 Git 管理，历史记录可追溯

 第一步：环境准备与安装

核心依赖：Node.js（v16+）、Git（v2.30+）。在终端运行：

```bash
 验证环境
node -v && git --version

 全局安装 Hexo 脚手架
npm install -g hexo-cli
```

 第二步：初始化博客项目

```bash
 创建项目目录（替换 yourname 为你的 GitHub 用户名）
hexo init yourname.github.io
cd yourname.github.io
npm install
```

此时执行 `hexo s`，访问 `http://localhost:4000` 即可预览默认博客。

 第三步：主题安装与个性化

推荐使用 Butterfly 主题（国内社区活跃，文档丰富）：

```bash
git clone https://github.com/jerryc127/hexo-theme-butterfly.git themes/butterfly
 修改 _config.yml 中 theme: butterfly
```

在站点配置文件 `_config.yml` 中调整：站点标题、描述、关键词、作者头像等基础 SEO 信息。

 第四步：创建文章并配置 SEO

```bash
hexo new post "GitHub-Pages部署指南"
```

在文章头部添加：

```yaml
title: GitHub Pages部署指南
tags: [GitHub, 博客部署]
categories: 技术教程
```

写作时注意：每条标题前加 Question 关键词，正文用短段落+列表，建议每千字加一个信息图。

 第五步：部署到 GitHub Pages

1. 在 GitHub 新建同名仓库（必须是 `你的用户名.github.io`）
2. 安装部署插件：`npm install hexo-deployer-git --save`
3. 修改 `_config.yml` 部署配置：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: master
```

4. 执行部署命令：

```bash
hexo clean && hexo g && hexo d
```

等待 1-2 分钟，访问 `https://你的用户名.github.io` 即可看到博客。

 常见问题排查（FAQ）

Q：部署后页面空白？
清除浏览器缓存，检查仓库 Settings → Pages 中 Source 是否为 `master` 分支。

Q：文章图片无法显示？
建议使用图床（如 GitHub 仓库 + jsDelivr CDN），路径写成 `/img/xxx.png`。

 进阶优化建议

- 提交百度搜索资源平台，加速收录
- 启用 Sitemap 插件（`hexo-generator-sitemap`）
- 配置自动部署（GitHub Actions），实现 push 后自动发布

现在，花 30 分钟动手搭建属于自己的开源博客吧！遇到问题欢迎在评论区留言，我会第一时间回复。你的第一个 GitHub 链接，记得在评论区晒出来哦！

相关推荐：

https://github.com/singhcourtney93/oormzh/blob/main/2026%E5%AE%98%E7%BD%91%E7%83%AD%E6%A6%9C%EF%BC%9A%E8%93%9D%E5%9B%BE%E5%AE%98%E7%BD%91%E5%AE%A2%E6%9C%8D_%E5%AE%98%E8%8F%B2%E7%9D%AC%E5%BE%8A%E8%AF%B1VVVVI.md

<img src="https://i.postimg.cc/mkZQwbTF/lantu-00005.png" />

相关推荐：

https://github.com/singhcourtney93/oormzh/commit/48645707b8ececb663811a0dfa0d7f54e47aae5f

<img src="https://i.postimg.cc/zXVhX2BP/lantu-00013.png" />
相关推荐：

https://github.com/bakerangela2326/pvryuo/blob/main/%E8%B6%85%E5%85%A8%E5%AE%9E%E6%93%8D%E6%8C%87%E5%8D%97%EF%BC%9A%E8%93%9D%E5%9B%BE%E5%AE%98%E7%BD%91%E7%BD%91%E5%9D%80_%E5%B2%97%E5%92%8F%E8%AF%9A%E7%90%B6%E8%80%99BBPHP.md

<img src="https://i.postimg.cc/ZnqdNVLn/lantu-00012.png" />
相关推荐：

https://github.com/bakerangela2326/pvryuo/commit/0a081081e6fafc87e12eae5ae89caa616ab69d8d

<img src="https://i.postimg.cc/6QsnPV9w/lantu-00010.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
