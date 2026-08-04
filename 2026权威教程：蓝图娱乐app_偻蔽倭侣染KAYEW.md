蓝图娱乐app【Q-——333307——】蓝图娱乐app【 辋芷《888yx●vip》 】
蓝图娱乐app【Q-——333307——】蓝图娱乐app【 辋芷《888yx●vip》 】

 从0到1搭建个人博客：GitHub Pages + Hexo 完整教程（2025亲测有效）

还在羡慕别人拥有独立博客？其实你离技术大佬只差一个 GitHub Pages。今天手把手教你用 Hexo 免费搭建高颜值博客，无需服务器，零成本，还能自定义域名。本文基于最新版 Node.js 20+ 和 Hexo 7 实测，跟着做一定能成功。

 第一步：环境准备与GitHub仓库创建

首先确保电脑已安装 Git 和 Node.js（建议LTS版本）。打开终端输入 `node -v` 验证安装。接着在 GitHub 新建仓库，仓库名必须为 `用户名.github.io`，这是 GitHub Pages 的硬性要求。勾选 Public 和 Add a README file，稍后我们会用 Git 命令推送本地文件。

```bash
 全局安装hexo命令行工具
npm install hexo-cli -g
```

 第二步：本地初始化Hexo项目

在你想存放博客的目录执行：

```bash
hexo init my-blog && cd my-blog
npm install
hexo server
```

浏览器访问 `http://localhost:4000`，看到默认页面说明初始化成功。此时目录结构中有 `source/_posts`（文章存放处）和 `_config.yml`（站点配置文件）。重点修改 `_config.yml` 中的 `url` 和 `title` 字段，否则部署后资源路径会报错。

 第三步：部署到GitHub Pages

安装部署插件：

```bash
npm install hexo-deployer-git --save
```

编辑 `_config.yml` 最底部：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```

执行 `hexo clean && hexo generate && hexo deploy`，稍等片刻访问 `用户名.github.io` 即可看到线上博客。遇到404？ 去仓库Settings→Pages页面把Branch切换为 `main`。

 第四步：写第一篇文章与常用命令

在 `source/_posts` 中新建 `.md` 文件，头部用 Front-matter 设置标题和标签：

```
---
title: 我的第一篇博客
tags: [新手教程]
date: 2025-01-01 12:00:00
---
```

写完后执行 `hexo g` 生成静态文件，`hexo d` 部署。建议养成 `hexo clean` 清除缓存的习惯，避免样式不同步。常用命令汇总：
- `hexo new "文章名"` 创建新文章
- `hexo server --draft` 本地预览草稿
- `hexo g -d` 生成并一键部署

---

互动引导：搭建过程中遇到任何报错（常见如端口被占用、Git认证失败），欢迎在评论区贴出错误代码，我会逐一解答。如果本文对你有帮助，点个 Star 或 在看，让更多朋友看到这份2025年最新实战指南。

关键词布局：GitHub Pages教程、Hexo搭建博客、免费博客部署、个人技术博客、静态网站生成器、Markdown写作、前端部署实践、DevOps入门。

---

本文已同步更新至我的博客，欢迎收藏转发。技术迭代快，建议关注公众号获取后续的「自动部署」「主题美化」进阶内容。

相关推荐：

https://github.com/gloverjoseph140/fniwrs/blob/main/%E8%BF%9B%E9%98%B6%E5%AE%9E%E6%93%8D%E6%8C%87%E5%8D%97%EF%BC%9A%E8%93%9D%E5%9B%BE%E5%BC%80%E6%88%B7%E6%B5%8B%E9%80%9F_%E7%9F%A3%E8%87%A3%E7%9A%84%E9%99%85%E5%8E%9DSGGAB.md

<img src="https://i.postimg.cc/rsg9XDf0/lantu-00001.png" />

相关推荐：

https://github.com/gloverjoseph140/fniwrs/commit/327ba296dbba93fc03d23b362c41d47f86bb7804

<img src="https://i.postimg.cc/6QsnPV9w/lantu-00010.png" />
相关推荐：

https://github.com/klinegina28/bhjqeg/blob/main/2026%E7%AC%AC%E4%B8%80%E8%A7%A3%E6%9E%90%EF%BC%9A%E8%93%9D%E5%9B%BE%E5%BC%80%E6%88%B7%E7%BD%91%E5%9D%80_%E7%96%91%E5%BE%97%E5%B7%B3%E6%B9%8D%E5%98%B6STGNC.md

<img src="https://i.postimg.cc/sfKP2ZJh/lantu-00007.png" />
相关推荐：

https://github.com/klinegina28/bhjqeg/commit/64a65cdd8816a14cf91a37bce2bb83f570171dd1

<img src="https://i.postimg.cc/FsWxTJds/lantu-00002.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
