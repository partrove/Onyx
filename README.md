# Onyx

Onyx 是一个简洁的 [Hugo](https://gohugo.io/) 主题，基于 [Archie](https://github.com/athul/archie) 修改而来。

Onyx 在 Archie 的基础上，精简了 Feather Icons 和英文字体，并引入了 [霞鹜文楷 Bright](https://chinese-font.netlify.app/zh-cn/fonts/lxgwwenkaibright/LXGWBright-Regular) 字体以优化中文显示。

## 安装

```bash
git clone https://github.com/partrove/Onyx.git themes/Onyx
```

## 配置

参考以下样例配置：

```toml
baseURL = 'https://blog.partrove.com/'
languageCode = 'zh-CN'
title = 'ParTrove'
theme = 'Onyx'

[languages]
  [languages.zh]
    languageCode = 'zh-CN'
    languageDirection = 'ltr'
    LanguageName = 'Chinese'
    weight = 1

[menus]
  [[menus.main]]
    name = '归档'
    pageRef = '/archives'
    weight = 10
  [[menus.main]]
    name = '分类'
    pageRef = '/categories'
    weight = 20
  [[menus.main]]
    name = '关于我'
    pageRef = '/about'
    weight = 30

[pagination]
  pagerSize = 6

[params]
  useCDN = true
[[params.social]]
name = "GitHub"
icon = "github"
url = "https://github.com/partrove/Onyx"
[[params.social]]
name = "X"
icon = "x"
url = "https://x.com/partrove"
```