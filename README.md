# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

## userテーブル

| column            | Type   | Options     |
| ----------------- | ------ | ------------|
| name              | string | null: false |
| self-introduction | text   |

Association

- has_many :tweets

## tweetsテーブル

| column            | Type   | Options     |
| ----------------- | ------ | ------------|
| photo             |
| map               | string  | null:false  |
| date              | integer | null: false |
| name              | string  | null: false |
| size              | integer |
| weight            | integer |
| congstion         | integer | null: false |
| toilet            | integer | null: false |
| fishing_shop      | integer | null: false |
| parking           | integer | null: false |
| memo              | text    | null: false |
| user              | references | foreign_key: true |

Association

- belongs_to :user
