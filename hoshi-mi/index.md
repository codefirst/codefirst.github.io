---
layout: product
canonical_url: http://www.codefirst.org/hoshi-mi/

title: Hoshi-mi
subtitle: A Heroku friendly visualization tool
copy: "You can make\nmany graphs easily"

description: |
  Hoshi-mi は、Heroku で動作することを重視したデータビジュアライゼーションツールです。
  同様のソフトウェアに GrowthForecast があります。

github_project: hoshi-mi
commiters: ["suer","mallowlabs","mzp"]

features:
 - name: Heroku 対応
   image: imgs/heroku.png
 - name: 簡単な API
   image: imgs/post.png
 - name: morris.js を利用した美しいグラフ
   image: imgs/morris.png
 - name: 複合グラフ対応
   image: imgs/complex.png

keywords: ["Ruby", "Heroku", "データビジュアライゼーション", "WebAPI"]
---

### GrowthForecast との比較

* Ruby on Rails 製であるため、一緒に使うことが多い Fluentd と親和性が高いです
* RRDTool を使っていません。RRDTool の生成するグラフに見飽きた方にぴったりです。
* Heroku 上で動作することを前提に作られています。そのため、リポジトリを push するだけですぐ使えます。
* API キーを知らなければデータを post できないように作られています。
* その他の機能は GrowthForecast よりも少ないです。

### ドキュメント

 * [マニュアル](https://readthedocs.org/docs/hoshi-mi/en/latest/)
