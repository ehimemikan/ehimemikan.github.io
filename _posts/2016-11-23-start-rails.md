# Ruby on Railsでなんか作ってみようと思った

[プロゲート](http://prog-8.com/)という初心者向けのプログラミング学習サイトが社内の非エンジニア間で流行っています。  
それはなんぞや、と体験してみようと思い、前から気になっていたRuby on Railsの学習をしてみました。  

あまりに簡単にWebサービスできるので、度肝を抜かれました。ほえー。  
kintoneのスピード感には勝てませんが、1からPHPとかで書くと話にならんですね。  

# Ruby on Railsをインストールする

https://www.oiax.jp/rails/zakkan/rails_4_2_installation_on_ubunt.html  
今だとこちらが親切でいい感じなんじゃないでしょうか。

で、軽く実行してみると。
```
$ rails new foo --skip-bundle
$ cd foo/
$ bundle install
$ rails g scaffold user name:string email:string
$ rake db:migrate
$ rails s
```
あとはこれで`http://localhost:3000/users`にアクセスするだけで簡単なユーザー登録ができるWebアプリ出来てました。ほえー。（2回目）  
じゃぁ、なんか作れないかやってみようかな、という気持ちになります。  
12月の社内ハッカソンまでに一通り触ってなんか形になるもの作っておきたいです。
