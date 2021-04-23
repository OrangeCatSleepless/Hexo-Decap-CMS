# hexo-netlify

## 介绍
使用[Hexo 5.4.0](https://hexo.io/)和[Netlify CMS](https://github.com/netlify/netlify-cms)构建的示例站点

使用子模块方式,目前内置[next主题 v8.3.0](https://github.com/next-theme/hexo-theme-next) | [fluid主题 v1.8.10](https://github.com/fluid-dev/hexo-theme-fluid) | [cards主题 1.1.0](https://github.com/ChrAlpha/hexo-theme-cards)

默认启用了[fluid主题](https://github.com/next-theme/hexo-theme-next),如要切换主题请在[_config.yml](https://github.com/leicancun/hexo-netlify/blob/main/_config.yml)更改`theme: fluid`中`fluid`改为你需要的主题名称


更多配置请查看对应主题自行修改

## 效果预览
![image-20210420211303684](https://gitee.com/leicancun/cdn/raw/master/Netlify-cms/image-20210420211303684.png)
![image-20210418222435713](https://gitee.com/leicancun/cdn/raw/master/Netlify-cms/image-20210418222435713.png)

![image-20210420212403763](https://gitee.com/leicancun/cdn/raw/master/Netlify-cms/image-20210420212403763.png)

支持在线修改主题配置

![image-20210420213142628](https://gitee.com/leicancun/cdn/raw/master/Netlify-cms/image-20210420213142628.png)

![image-20210420214308165](https://gitee.com/leicancun/cdn/raw/master/Netlify-cms/image-20210420214308165.png)

![image-20210418223337304](https://gitee.com/leicancun/cdn/raw/master/Netlify-cms/image-20210418223337304.png)

[后台管理预览](https://qwqmiao.cf/admin/)

### Netlify CMS编辑器工作流程

已在存储库中设置了Netlify CMS`admin`面板。您可以通过“ yourwebsite.com/admin”（例如“ localhost：4000 / admin”）访问它。**如提示配置错误请写死路径`/admin/`**,如"yourwebsite.com/admin/"。
要了解有关配置的更多信息，请查看[Netlify CMS docs](https://www.netlifycms.org/docs/intro/)。

## 食用方案

详细介绍文章请查看👉[Hexo Netlify CMS:在线编辑博客文章和配置](https://www.myql.xyz/post/8f487fbb/)

### 部署到Netlify

使用以下部署按钮启动并运行您自己的存储库副本：

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/leicancun/hexo-netlify&stack=cms)

部署到Netlify按钮会将此存储库的副本克隆到您自己的GitHub或GitLab帐户。

### 部署到Vercel

需要自己修改并配置才能正常使用`netlify cms`

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/leicancun/hexo-netlify.git)

## 待改进

由于对`css`不是熟悉，尚未配置页面自适应，编辑界面下预览效果不佳，手机等设备显示效果差，等待优化。

### 参考:
https://github.com/lunaceee/hexo-material-netlify