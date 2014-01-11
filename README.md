# Light-Kai

[Hexo] Theme Mod By Niphor

只是自用，还没改完，我很懒

## Install

Execute the following command and modify `theme` in `_config.yml` to `light-kai`.

```
git clone git://github.com/niphor/hexo-theme-light-kai.git themes/light-kai
```

## Update

Execute the following command to update Light.

```
cd themes/light-kai
git pull
```

## Config

Default config:

``` yaml
menu:
  首页: /
  归档: /archives

widgets:
- search
- category
- tag

excerpt_link: 详细
fancybox: true
rss: /atom.xml

#分享插件
share_provider: baidu

##addthis插件
share_addthis:
  enable: true
  pubid:
  facebook: true
  twitter: true
  google: false
  pinterest: false

##baidu分享定制的太多，直接拷贝代码到 layout/share/baidu.ejs里面

twitter:
  username: 
  show_replies: false
  tweet_count: 5


#评论插件
comment_provider: duoshuo

##Facebook comment
comment_facebook:
  appid: 123456789012345
  comment_count: 5
  comment_width: 840
  comment_colorscheme: light

##多说评论组件
comment_duoshuo: 
  short_name: niphor-dev

google_analytics:
```

- **menu** - Main navigation menu
- **widget** - Widgets displaying in sidebar
- **excerpt_link** - "Read More" link text at the bottom of excerpted articles
- **fancybox** - Enable [Fancybox]
- **rss** - RSS subscription link (change if using Feedburner)
- **share_provider** Share buttons provider
- **share_addthis** - Share buttons at the buttom of articles (Powered by [AddThis])
  - **enable** - Enable share buttons
  - **pubid** - Profile ID of [AddThis]
  - **facebook** - Enable Facebook button
  - **twitter** - Enable Twitter button
  - **google** - Enable Google+ button
  - **pinterest** - Enable Pinterest button
- **twitter** - Twitter widget config
  - **username** - Twitter username
  - **show_replies** - Enable displaying replies
  - **tweet_count** - Tweets display in widget
- **comment_provider** Comment Function provider
- **comment_facebook** - Comment Function (Powered by [Facebook])
  - **appid** - Facebook App ID
  - **comment_count** - Comment Number to Show
  - **comment_width** - Comment Dialog Width
  - **comment_colorscheme** - Comment Dialog Theme
- **comment_duoshuo** - Comment Function (Powered by [多说])
  - **short_name** - Your DuoShuo Short Name 
- **google_analytics** - Google Analytics ID

##Changelog

2014-01-11

1.  change jquery/imageresize/fancybox load from cdnjs,may slower in china
2.  addthis replaced with baidu share by default
3.  disqus replaced with duoshuo by default 
4.  change h1-h6/blockquote style in article
5.  not excute js if there is no photo in .gallery  


[Hexo]: http://zespia.tw/hexo/
[AddThis]: https://www.addthis.com
[多说]: https://www.duoshuo.com.com
[Facebook]: https://www.facebook.com
