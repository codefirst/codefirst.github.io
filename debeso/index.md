---
layout: product
canonical_url: http://www.codefirst.org/debeso/

title: debeso
subtitle: 開発者向けスニペットストック
copy: "Stock\nYour\nKnowledge"

description: |
  debeso は、開発者向けのスニペットストックです。
  開発者間の知識を共有し、知識が行方不明になることを防ぎます。

github_project: debeso
commiters: ["mallowlabs", "suer"]

features:
 - name: バージョン管理
   image: imgs/ss_version.png
 - name: シンタックスハイライト
   image: imgs/ss_syntax.png
 - name: API
   image: imgs/ss_api.png
 - name:  高速検索
   image: imgs/ss_search.png

keywords: ["スニペット", "Gist", "debeso"]
---

### 動作環境

 * Ruby 1.8+
 * RubyGems 1.4.2+
 * Bundler 1.0.15+
 * SQLite 3.6.18+
 * Git 1.4.7.1+

### インストール

[ダウンロードページ](https://github.com/codefirst/debeso/tags)から最新版をダウンロードし、展開してください。展開したディレクトリを debeso にリネームし、 以下のコマンドを実行してください。

{% highlight bash %}
$ cd debeso
$ cp config/settings.yml.example config/settings.yml
$ vi config/settings.yml
$ bundle install --path vendor/bundle
$ bundle exec padrino rake ar:migrate
$ bundle exec padrino start
{% endhighlight %}

インストールが完了したら[http://localhost:3000/](http://localhost:3000/)にアクセスしてください。

### デモサイト

 * [debeso on Heroku](https://debeso.herokuapp.com/)

一定時間が経過するとリポジトリは自動で削除されます。
