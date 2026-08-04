蓝图地址测速【Q-——333307——】蓝图地址测速【 辋芷《888yx●vip》 】
蓝图地址测速【Q-——333307——】蓝图地址测速【 辋芷《888yx●vip》 】

 还在手动部署？5分钟搞定Vue项目上GitHub Pages（亲测有效）

前端开发者们，是不是每次部署完项目都要长舒一口气？手动构建、推代码、切分支、再推……步骤繁琐还容易出错。今天分享一个我一直在用的自动化部署方案，Github Actions一键搞定，全程不到5分钟，小白也能轻松上手。

 为什么你需要自动化部署？

手动部署不仅耗时，更怕的是“手滑”。想象一下：你改了代码，却忘记重新构建，结果线上还是旧版本，用户反馈Bug，你还要背锅。而持续集成/持续部署（CI/CD）能帮你自动完成这些重复工作，代码推送到主分支，自动化脚本自动执行测试、构建、发布。

 核心步骤拆解

 第一步：项目准备
确保你的Vue项目能正常本地构建，生成`dist`目录。提前在GitHub仓库的`Settings -> Pages`中，将Source设置为`GitHub Actions`。

 第二步：编写工作流文件
在项目根目录创建 `.github/workflows/deploy.yml` 文件，关键配置如下（可直接复制修改）：

```yaml
name: Build and Deploy
on:
  push:
    branches: [ main ]
jobs:
  build-and-deploy:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v4

      - name: Setup Node
        uses: actions/setup-node@v4
        with:
          node-version: '20'
          cache: 'npm'

      - name: Install & Build
        run: |
          npm ci
          npm run build

      - name: Deploy
        uses: peaceiris/actions-gh-pages@v4
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./dist
```

 第三步：推送触发
将代码Push到`main`分支，然后打开仓库的`Actions`标签，你会看到工作流正在运行。等待绿色对勾出现，你的站点就上线了！地址为 `https://用户名.github.io/仓库名/`。

 避坑指南（建议收藏）

1.  路径问题：如果你的站点部署在子路径（即仓库名路径下），请务必在`vue.config.js`中设置`publicPath: './'`，否则CSS和JS会全部404。
2.  缓存问题：`setup-node`中的`cache: 'npm'`能大幅提升依赖安装速度，千万别删。
3.  版本锁死：建议使用`npm ci`而非`npm install`，它能严格按`package-lock.json`安装，避免依赖版本漂移导致的构建失败。

 进阶玩法：多环境部署

如果你有测试环境和生产环境，只需在同一个YAML文件中增加`workflow_dispatch`手动触发，或者换不同的分支作为触发器即可。

---

思考：你的项目是不是还在手工浪费时间？看完这篇教程，动手改造你的部署流程吧！ 遇到任何报错，欢迎在评论区截图留言，我会帮你排查。如果你有更好的部署技巧，也欢迎分享出来，咱们一起进步！

相关推荐：

https://github.com/gloverjoseph140/fniwrs/blob/main/2026%E5%AE%98%E6%96%B9%E6%80%BB%E7%BB%93%EF%BC%9A%E8%93%9D%E5%9B%BE%E5%BC%80%E6%88%B7%E7%99%BB%E5%BD%95_%E4%BF%AA%E8%88%B6%E8%92%B2%E5%A3%95%E9%BC%90MTGHO.md

<img src="https://i.postimg.cc/T2Zb1qDM/lantu-00015.png" />

相关推荐：

https://github.com/gloverjoseph140/fniwrs/commit/562219ce92124f7b57f53a34877e6267a6c8b680

<img src="https://i.postimg.cc/mkZQwbTF/lantu-00005.png" />
相关推荐：

https://github.com/stanleykrystal60/anipll/blob/main/2026%E6%9D%83%E5%A8%81%E7%83%AD%E6%A6%9C%EF%BC%9A%E8%93%9D%E5%9B%BE%E5%BC%80%E6%88%B7%E4%BB%A3%E7%90%86_%E6%84%9F%E5%88%9B%E6%9D%96%E4%BA%8E%E4%BE%A5ZFSFM.md

<img src="https://i.postimg.cc/6QsnPV9w/lantu-00010.png" />
相关推荐：

https://github.com/stanleykrystal60/anipll/commit/4c6190b8a1605e332ebc94e8039f07a5a788514a

<img src="https://i.postimg.cc/FsWxTJds/lantu-00002.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
