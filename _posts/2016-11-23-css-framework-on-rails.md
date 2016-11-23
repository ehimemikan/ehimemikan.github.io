---
layout: post
title:  "Ruby on RailsのCSSフレームワーク"
date:   2016-11-23 08:10:00 +0900
categories: jekyll update
---

# Railsで使えるフレームワークを考える

有名どころを調べます。

* Bootstrap
* Materialize
* uikit
* Pure

## [Bootstrap](http://getbootstrap.com/)

言わずと知れた、超有名なフレームワークです。  
が、個人的にはやや見るのに飽きましたし、すこし古いイメージがあります。  
あと、結構巨大です。

## [Materialize](http://materializecss.com/)

良さそう！って思ったのはこれでした。  
ただ、これjQueryが必須なんですよね。  
ちょっとjQueryはJavaScriptを考えるときにあんまり入れたくなかったので、今回はパスします。  

## [uikit](https://getuikit.com/index.html)

うーん。  
これもjQueryが必要そう。  

## [Pure](http://purecss.io/)

軽量系。  
公式サイトの感じもかなり好きなんですが、どうも2015年2月を最後に更新が止まっている...。  

# 最終的にどうする

[Rails + React + Material-UI](https://rubyonrails4makeitwork.wordpress.com/2016/04/11/rails-react-material-ui/)

これで行ってみます。  
さっきjQueryをパスした理由は、Reactを使いたかったから、邪魔なものは入れたくなかったんです。  

[Material-UI](http://www.material-ui.com/)  

Material-UIの最新が`v0.16.2`だったので、`package.json`のところは変更しました。  
加えて、`react`は`~15.3.0`に変更しました。  
理由は、  

```
├─┬ material-ui@0.16.4  
│ ├── lodash.merge@4.6.0  
│ ├── lodash.throttle@4.1.1  
│ └─┬ react-event-listener@0.4.0  
│   └── react-addons-shallow-compare@15.4.0  
├── UNMET PEER DEPENDENCY react@15.4.0  
└── UNMET PEER DEPENDENCY react-tap-event-plugin@0.2.2  
```

となってしまったからです。
