# hexo-netlify

## 介绍
使用[Hexo 5.2.0](https://hexo.io/)和[Netlify CMS](https://github.com/netlify/netlify-cms)构建的示例站点

目前内置[next主题 v8.0.1](https://github.com/next-theme/hexo-theme-next) | [fluid主题 v1.8.4](https://github.com/fluid-dev/hexo-theme-fluid) | [cards主题 1.1.0](https://github.com/ChrAlpha/hexo-theme-cards)

默认启用了[next主题](https://github.com/next-theme/hexo-theme-next),如要切换主题请在[_config.yml](https://github.com/leicancun/hexo-netlify/blob/main/_config.yml)更改`theme: next`中`next`改为你需要的主题名称


更多配置请查看对应主题自行修改

## 效果预览
![效果预览图](https://gitee.com/leicancun/img/raw/main/hexo-Netlify/Snipaste_2020-10-18_13-39-38.png)
![效果预览图2](https://gitee.com/leicancun/img/raw/main/hexo-Netlify/Snipaste_2020-10-18_13-40-04.png)

[后台管理预览](https://qwqmiao.cf/admin/)

### Netlify CMS编辑器工作流程

已在存储库中设置了Netlify CMS`admin`面板。您可以通过“ yourwebsite.com/admin”（例如“ localhost：4000 / admin”）访问它。**如提示配置错误请写死路径`/admin/`**,如"yourwebsite.com/admin/"。
要了解有关配置的更多信息，请查看[Netlify CMS docs](https://www.netlifycms.org/docs/intro/)。

## 食用方案

### 部署到Netlify

使用以下部署按钮启动并运行您自己的存储库副本：

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/leicancun/hexo-netlify&stack=cms)

部署到Netlify按钮会将此存储库的副本克隆到您自己的GitHub或GitLab帐户。

### 部署到Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/leicancun/hexo-netlify.git)

### 参考:
https://github.com/lunaceee/hexo-material-netlify