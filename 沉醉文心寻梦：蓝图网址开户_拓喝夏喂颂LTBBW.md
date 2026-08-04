蓝图网址开户【Q-——333307——】蓝图网址开户【 辋芷《888yx●vip》 】
蓝图网址开户【Q-——333307——】蓝图网址开户【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程

你是否想过拥有一个完全属于自己的技术博客？没有广告、自由定制、永久免费——GitHub Pages 搭配 Hexo 就是最佳解决方案。本文将手把手教你从零开始，30分钟上线你的第一个个人网站。

 为什么选择 GitHub Pages + Hexo？

GitHub Pages 提供免费静态托管，支持自定义域名，全球访问速度快。Hexo 是目前最流行的静态博客框架，基于 Node.js，操作简单，主题丰富。

相比 WordPress 或 CSDN，这套方案的优势明显：
- 完全免费，无需服务器
- 支持 Markdown 写作，专注内容创作
- 代码开源，可深度定制
- 自动部署，Git 推送即更新

 环境准备：3个必需工具

开始前，请确保电脑已安装：
1. Git：版本控制工具，[下载地址](https://git-scm.com/)
2. Node.js：运行环境，建议 LTS 版本，[下载地址](https://nodejs.org/)
3. GitHub 账号：注册一个，免费

安装完成后，打开终端（Mac/Linux）或 CMD（Windows），输入 `git --version` 和 `node -v` 验证是否成功。

 快速部署：5步上线博客

 第一步：安装 Hexo
```bash
npm install -g hexo-cli
```

 第二步：初始化博客项目
```bash
hexo init my-blog
cd my-blog
npm install
```

 第三步：本地预览
```bash
hexo server
```
浏览器访问 `http://localhost:4000`，看到默认博客即成功。

 第四步：创建首篇文章
```bash
hexo new "我的第一篇文章"
```
用文本编辑器打开 `source/_posts/` 下的 .md 文件，写入内容，保存后刷新浏览器即可预览。

 第五步：部署到 GitHub
1. 在 GitHub 新建仓库，命名为 `你的用户名.github.io`
2. 修改根目录 `_config.yml` 文件，在末尾添加：
```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```
3. 安装部署插件并推送：
```bash
npm install hexo-deployer-git --save
hexo clean && hexo generate && hexo deploy
```

稍等1-2分钟，访问 `https://你的用户名.github.io`，你的博客就上线了！

 个性化配置：3个关键优化

1. 更换主题：在 [Hexo Themes](https://hexo.io/themes/) 挑选热门主题，如 Next、Fluid，下载后放入 `themes/` 目录，修改 `_config.yml` 中的 `theme` 字段。

2. 添加搜索与标签：安装插件 `hexo-generator-searchdb` 和 `hexo-generator-tag`，让文章更容易被发现。

3. 绑定域名：购买域名后在 GitHub 仓库 Settings → Pages 中填写，再到域名服务商添加 CNAME 记录，即可用专属域名访问。

 常见问题与解决

- 部署失败：检查仓库名是否完全匹配，GitHub 现在默认分支为 main。
- 图片不显示：Hexo 中图片需放在 `source/images/` 下，或使用 `{% asset_img 文件名 %}` 标签。
- 本地正常但线上404：执行 `hexo clean` 后重新部署。

 进阶：让博客更好用

- 使用 GitHub Actions 实现推送自动部署
- 配置 Travis CI 实现多分支管理
- 添加 评论系统（如 Gitalk、Valine）

 写在最后

现在，你已经拥有了一个完全属于自己的技术博客。坚持写作，分享你的学习心得与项目经验，它会成为你技术成长的最佳见证。

遇到问题？欢迎在评论区留言，或加入 Hexo 中文社区（`hexo-china`）获取帮助。如果本文对你有用，请点赞、收藏并分享给需要的朋友，你的支持是我持续输出的动力！

关注我，获取更多技术干货与效率工具推荐。下一篇，我们将聊聊“如何用 GitHub Actions 自动部署博客”，敬请期待！

相关推荐：

https://github.com/bakerangela2326/pvryuo/blob/main/2026%E7%A7%91%E6%8A%80%E7%88%86%E7%82%B9%EF%BC%9A%E8%93%9D%E5%9B%BE%E5%AE%98%E6%96%B9%E4%B8%8B%E8%BD%BD_%E7%A7%98%E5%95%84%E8%88%B6%E8%B0%92%E6%BD%AEUOHVC.md

<img src="https://i.postimg.cc/rsg9XDf0/lantu-00001.png" />

相关推荐：

https://github.com/bakerangela2326/pvryuo/commit/d3cdc8e17fb9658ad9a5b01ecb9ef9967205142c

<img src="https://i.postimg.cc/9fTtX8xf/lantu-00003.png" />
相关推荐：

https://github.com/benderjessica393/clipwq/blob/main/2026%E6%9D%83%E5%A8%81%E6%95%99%E7%A8%8B%EF%BC%9A%E8%93%9D%E5%9B%BE%E5%AE%98%E6%96%B9%E6%B5%8B%E9%80%9F_%E8%A9%B9%E5%A5%B6%E8%AF%92%E5%92%8F%E7%82%AEICQEY.md

<img src="https://i.postimg.cc/9fTtX8xf/lantu-00003.png" />
相关推荐：

https://github.com/benderjessica393/clipwq/commit/c0b1c961269e8274fc1cdfab7b6eb8e2312aec43

<img src="https://i.postimg.cc/kGjWYk5W/lantu-00006.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
