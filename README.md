# hexo-netlify

## 介绍
使用[Hexo](https://hexo.io/)和[Netlify CMS](https://github.com/netlify/netlify-cms)构建的示例站点,默认主题为[Next](https://github.com/next-theme/hexo-theme-next)

[网站预览](https://raingking.eu.org/)

[后台管理预览](https://raingking.eu.org/admin/#/)

### Netlify CMS编辑器工作流程

已在存储库中设置了Netlify CMS`admin`面板。您可以通过“ yourwebsite.com/admin”（例如“ localhost：4000 / admin”）访问它。
要了解有关配置的更多信息，请查看[Netlify CMS docs](https://www.netlifycms.org/docs/intro/)。

## 食用方案

### 部署到Netlify

使用以下部署按钮启动并运行您自己的存储库副本：

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/leicancun/hexo-netlify&stack=cms)

部署到Netlify按钮会将此存储库的副本克隆到您自己的GitHub或GitLab帐户。

### 部署到Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/leicancun/hexo-netlify.git)

### 资源目录:
```
root
 ├── package.json  应用程序的信息
 ├── scaffolds  模版文件夹,一般不用动
 │   ├── draft.md
 │   ├── page.md
 │   └── post.md
 ├── source  各种资源文件,一般修改主要改这里
 │   ├── admin  CMS配置
 │   │   ├── config.yml
 │   │   └── index.html
 │   ├── categories  分类
 │   │   └── index.md
 │   ├── tags  标签
 │   │   └── index.md
 │   ├── _data  数据
 │   │   ├── head.njk
 │   │   └── next.yml
 │   └── _posts  文章
 │       └── hello-world.md
 ├── themes  主题文件夹
 │   ├── landscape  hexo默认主题
 │   └── next  next主题
 └── _config.yml 站点配置
```
### _config.yml
配置文件位置`root/__config.yml`

已配置永久链接和本地搜索
```
# 永久链接
abbrlink:
  alg: crc32  #support crc16(default) and crc32
  rep: hex    #support dec(default) and hex
  drafts: false #(true)Process draft,(false)Do not process draft
  # Generate categories from directory-tree
  # depth: the max_depth of directory-tree you want to generate, should > 0
  auto_category:
     enable: true
     depth:

# 本地搜索
search:
  path: search.xml
  field: post
  format: html
  limit: 100
```

### next.yml

配置文件位置`source/_data/next.yml`

已启用配置:

- 自定义文件路径

      custom_file_path:
      head: source/_data/head.njk

- 黑暗模式:开

      darkmode: true

- 已添加了首页、标签、归档页面

  menu:
    
	  home: / || fa fa-home  首页  
	  tags: /tags/ || fa fa-tags  标签   
	  archives: /archives/ || fa fa-archive  归档

- 侧边栏位置改为右侧

      sidebar:
      #position: left  左
      position: right  右

- 侧边栏社交链接添加管理员页面

      Social Links
      social:
      Admin: https://raingking.eu.org//admin || fas fa-leaf

  将其中的 `raingking.eu.org`换成你自己的域名,图标不满意也可以自己去修改

- 修改默认代码样式，开启复制按钮

  codeblock:
  
      theme:
	  light: solarized-light
      copy_button:
	  enable: true

  Available values: default | flat | mac

      style: mac

- 开启返回顶部按钮百分比显示

  back2top：

      scrollpercent：true

- 开启pjax

      pjax: true

- 开启懒加载

      lazyload: true

- 开启预加载

      quicklink:
      enable: true

- 开启搜索

      local_search:
      enable: true

- 关闭过度动画并修改外部库为jsdelivr

      motion:
      enable: false

      vendors:
      internal: jsdelivr
  如果直接修改外部库不关动画会导致看不见文章，不知道是不是bug

###  head.njk

配置文件位置`source/_data/head.njk`

已添加**网页点击特效**和**网页标题崩溃**并默认启用如需关闭请添加`<!-- -->`注释

``` html
<script defer="true" type="text/javascript"    src="//cdn.jsdelivr.net/combine/gh/leicancun/JSCDN/js/crash_cheat.min.js,gh/leicancun/JSCDN/js/fireworks.min.js"></script>
```

已添加看板娘,默认未启用,如需启用请去掉注释`<!-- -->`

```html
<!-- <script defer="true" src="//cdn.jsdelivr.net/gh/leicancun/live2d-widget@0.8.1/autoload.min.js"></script> -->
```

### 参考:
https://github.com/lunaceee/hexo-material-netlify