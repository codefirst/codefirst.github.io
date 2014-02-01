---
layout: product
canonical_url: http://www.codefirst.org/sunline/

title: Sunline
subtitle: A lightweight script and log management tool
copy: "Let's start DevOps from\na small first step"

description: |
  Sunline は本番サーバでのスクリプトの実行とログの管理を行うシンプルな Web アプリケーションです。
  同様のソフトウェアに Webistrano があります。

github_project: sunline
commiters: ["suer","mallowlabs"]

features:
 - name: スクリプトの集中管理
   image: imgs/script.png
 - name: 実行はワンライナー
   image: imgs/oneliner.png
 - name: サーバ毎の実行ログ
   image: imgs/log.png
 - name: WebHook 対応
   image: imgs/webhook.png

keywords: ["Heroku", "DevOps", "Webistrano", "Ruby"]
---

### Webistrano との比較

* スクリプトは、Capistrano ではなくシェルスクリプトで記述するため、学習コストを低く抑えられます。
* サーバにログイン後にスクリプトを実行する形式なので、秘密鍵等の設定が不要です。
* スクリプトを Web アプリケーションに直接記述する形式のため、バージョン管理システムの知識が不要です。
* 添付ファイルも Web アプリケーションにアップロードする方式です。
* サーバやロールの管理機能はありません。

