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
