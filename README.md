# Depot for rails 3.2.22.5

## 概要

- 書籍 　「RailsによるアジャイルWebアプリケーション開発（第４版）のサンプル(depot)です。

## 動作環境

- os: macOS 10.12.6
- Ruby 1.9.3-p551
- Rails 3.2.22.5

## 実装手順

```
$ git clone https://github.com/sinya-otonari/depot
$ cd depot
$ bundle install
$ rake db:migrate
$ rake db:migrate RAILS_ENV=test
$ rake db:seed
$ RUBYOPT=-W0 rake test
$ rails server
```

## 実装内容

- 2017/07/12 第6章 タスクA：アプリケーションの作成
- 2017/08/02 第7章 タスクB：検証とユニットテスト
- 2017/08/23 第8章 タスクC：カタログの表示
- 2017/08/30 第9章 タスクD：カートの作成
- 2017/09/06 第10章 タスクE：もっとスマートなカート
- 2017/10/04 第11章 タスクF：Ajax の追加
- 2017/10/25 第12章 タスクG:チェックアウト
  - p163の修正コード(orders_controller.rb)
  ```
  変更前#@orders = Order.paginate :page=>params[:page], :order=>'created_at desc',
  :per_page => 10
  変更後@orders = Order.page(params[:page]).order('created_at desc').per_page(10)
  ```
- 2017/11/15 第13章 タスクH：メールの送信
- 2018/01/17 第14章 タスクI：ログイン
