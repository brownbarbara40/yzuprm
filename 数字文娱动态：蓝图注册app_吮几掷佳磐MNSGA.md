蓝图注册app【Q-——333307——】蓝图注册app【 辋芷《888yx●vip》 】
蓝图注册app【Q-——333307——】蓝图注册app【 辋芷《888yx●vip》 】

 从零搭建个人博客：我用GitHub Pages + Hexo实现了自动化部署

> 你是否也想过拥有一个属于自己的技术博客？不依赖第三方平台，完全掌控内容和样式？这篇文章记录了我从零开始，用GitHub Pages和Hexo搭建个人博客的全过程，并实现了自动化部署。文末有完整资源清单，记得看到最后。

 为什么选择GitHub Pages搭建博客？

GitHub Pages是GitHub提供的免费静态网站托管服务，它有几个核心优势：

- 完全免费，无需购买服务器和域名
- 支持自定义域名，也可以使用默认的username.github.io
- 自带HTTPS加密，安全可靠
- 与Git工作流无缝集成，推送代码即完成发布

对于开发者来说，这几乎是零成本搭建个人品牌的最佳选择。

 核心工具链：Hexo + GitHub Actions

 Hexo：轻量级静态博客框架

Hexo是一个基于Node.js的快速、简洁且高效的博客框架。它支持Markdown语法，可以一键生成静态页面。安装只需要三步：

```bash
npm install -g hexo-cli
hexo init my-blog
cd my-blog && npm install
```

 GitHub Actions：自动化部署流水线

这是整个流程中的点睛之笔。通过配置工作流文件，我实现了“本地写文章，推送即发布”的自动化流程。核心配置片段如下：

```yaml
- name: Deploy
  uses: peaceiris/actions-gh-pages@v3
  with:
    github_token: ${{ secrets.GITHUB_TOKEN }}
    publish_dir: ./public
```

 三步完成博客搭建

第一步： 创建仓库并命名为`username.github.io`（username替换为你的GitHub用户名）。

第二步： 在本地完成Hexo初始化，修改`_config.yml`中的主题、标题等基础配置。

第三步： 推送代码到主分支，GitHub Actions会自动构建并部署到Pages服务。

 一个容易忽略的优化细节

使用CDN加速静态资源，将博客的图片、CSS和JS文件上传到图床或使用jsDelivr加速，能显著提升国内访问速度。我实际测试发现，开启CDN后页面加载时间从3秒降到了0.8秒。

 互动环节

你在搭建博客时遇到过什么Bug？或者有什么独特的优化技巧？欢迎在评论区分享你的经验，我会逐一回复。

如果这篇文章对你有帮助，点赞、收藏、关注是我持续输出的最大动力。后续我会更新关于SEO优化和自定义主题的进阶教程。

---

资源清单（长按复制到浏览器访问）：
- Hexo官方文档：hexo.io/zh-cn/docs
- GitHub Pages指南：pages.github.com
- 免费CDN加速：www.jsdelivr.com

相关推荐：

https://github.com/benderjessica393/clipwq/blob/main/2026%E7%A7%91%E6%8A%80%E5%B9%B2%E8%B4%A7%EF%BC%9A%E8%93%9D%E5%9B%BE%E4%B8%BB%E7%AE%A1%E7%BD%91%E5%9D%80_%E6%92%AC%E8%8F%9C%E8%B4%9F%E5%88%B0%E8%8D%B7EPNNQ.md

<img src="https://i.postimg.cc/9fTtX8xf/lantu-00003.png" />

相关推荐：

https://github.com/benderjessica393/clipwq/commit/aa91562cd4213e1d2da32644fcc09e3b797a9a97

<img src="https://i.postimg.cc/ZnqdNVLn/lantu-00012.png" />
相关推荐：

https://github.com/orozcogregory68/fxoxig/blob/main/2026%E7%AC%AC%E4%B8%80%E7%83%AD%E6%A2%97%EF%BC%9A%E8%93%9D%E5%9B%BE%E4%B8%BB%E7%AE%A1%E7%99%BB%E5%BD%95_%E6%AF%96%E6%8C%A0%E8%B0%A1%E9%97%BB%E5%8F%82MMZBB.md

<img src="https://i.postimg.cc/ZnqdNVLn/lantu-00012.png" />
相关推荐：

https://github.com/orozcogregory68/fxoxig/commit/787ee50b38de6b07ebfa6ec6251bf3b19d7851cd

<img src="https://i.postimg.cc/kGjWYk5W/lantu-00006.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
