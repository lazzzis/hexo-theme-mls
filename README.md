# hexo-theme-mls

A hexo made for hexo3

[Preview](https://lazzzis.github.io/hexo-theme-mls)

## Installation

1. Clone
   `git clone https://github.com/lazzzis/hexo-theme-mls.git`

2. Install some plugins on your blog root directory

   `npm install --save hexo-image-caption`

3. Revise `_config.yml` in your blog root directory

   ```yaml
   theme: hexo-theme-mls # enable the theme

   highlight: # disable default highlight
     enable: false
     line_number: false
     auto_detect: false

   # add caption for iamges
   image_caption:
     enable: true #false to disable
   ```

4. Tags and categories

   Create two folders under your `source` directory: `tags` and `categories`.

   Create an `index.md` file under each folder that you've just created.

   `tags/index.md`:

   ```
   layout: tags
   title: tags
   ---
   ```

   `categories/index.md`:

   ```
   layout: categories
   title: categories
   ---
   ```

## Config

1. the `_config.yml` in this theme folder

   ```yaml
   # Header
   menu:
     Home: /
     Archives: /archives
     Categories: /categories
     Tags: /tags
     Links: /links
     About: /about
   rss: /atom.xml

   # Google Analytics

   google_analytics:

   # Miscellaneous
   favicon: # url for your favicon
   twitter: # twitter id
   github: # github id
   fb_app_id:
   instagram:
   music: # your id in music.163.com, like http://music.163.com/#/user/home?id=...

   # due to some reason, this has to be a url rather than id
   google_plus:

   # disable some share applications.
   # For the details of all the applications, please refer to https://github.com/overtrue/share.js
   share_disabled: weibo,qzone,qq,tencent,douban,linkedin,diandian
   ```

2. background image

   The image is under `source/css/images`, and it has to be named as 'background.jpg';
