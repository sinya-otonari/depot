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
