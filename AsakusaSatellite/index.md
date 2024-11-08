---
layout: product
canonical_url: https://www.codefirst.org/AsakusaSatellite/

title: AsakusaSatellite
subtitle: 開発者向けリアルタイムチャットアプリケーション
copy: "コミュニケーションを\n加速する\nAsakusaSatellite"

description: |
  AsakusaSatellite は、開発者向けのリアルタイムチャットアプリケーションです。
  開発者間のコミュニケーション品質を向上し、ソフトウェア開発にリズムをもたらします。

github_project: AsakusaSatellite
commiters: ["mallowlabs", "suer", "mzp", "shimomura1004", "banjun"]

features:
 - name: リアルタイムコミュニケーション
   image: imgs/ss_realtime.png
 - name: プラグインによる拡張
   image: imgs/ss_plugin.png
 - name: ソースコードのシンタックスハイライト
   image: imgs/ss_code.png
 - name: iPhone UI
   image: imgs/ss_iphone.png
 - name: Redmine のチケットリンク
   image: imgs/ss_ticket_link.png
 - name: 全文検索
   image: imgs/ss_search.png

keywords: ["チャットアプリケーション", "Rails", "WebSocket"]
---

### 動作環境

 * Ruby 1.8.7 / 1.9.3 / 2.0.0 / 2.1.0 or JRuby 1.7.1
 * RubyGems 1.4.2 or later
 * Bundler 1.0.7 or later
 * MongoDB 1.8.1 or later
 * Google Chrome / Firefox / Safari

### インストール

[ダウンロードページ](https://github.com/codefirst/AsakusaSatellite/tags) から最新版をダウンロードし、展開してください。
展開したディレクトリを AsakusaSatellite にリネームし、以下のコマンドを実行してください。

{% highlight bash %}
$ cd AsakusaSatellite

# 依存ライブラリのインストール
$ bundle install --path .bundle --without development test

# MongoDB と Socky の起動
$ mongod --dbpath /path/to/db
$ bundle exec thin -R socky/config.ru -p3002 -t0 start

# AsakusaSatellite の起動
$ bundle exec rake assets:precompile RAILS_ENV=production
$ bundle exec rails server -e production
{% endhighlight %}

インストールが完了したら [http://localhost:3000/](http://localhost:3000/) にアクセスしてください。

### ドキュメント

 * [ブログ記事](http://blog.codefirst.org/tagged/AsakusaSatellite)
 * [発表資料 (名古屋 Reject 会議 02)](https://www.slideshare.net/mallowlabs/a-realtime-chat-application-for-developers-asakusasatellite)
 * [発表資料 (LL 名古屋)](https://www.slideshare.net/suer81/how-are-asakusasatellite-growing-with-mzp)
