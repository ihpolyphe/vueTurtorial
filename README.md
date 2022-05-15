# VueTurtorial

フロントエンドの勉強をして NodeJsMySQLHeroku のフロントエンドを改良したい

## Vue.js のセットアップ

- Vue.js インストール
  sudo npm install -g @vue/cli@next

- Vue ディレクトリ 環境構築
  vue create todo-list
  cd todo-list
- 以下でサーバ立てる
  npm run serve
  http://localhost:8080/ にアクセス

- Vuex インストール
  npm install vuex@next --save

## 参照

[Vue 初学者のための TodoList チュートリアル【入門】](https://tech-blog.rakus.co.jp/entry/20210910/vue)

## 動かし方

- ToDo の json ファイルをサーバとして立ち上げ
  cd /mnt/c/Users/xxx/Desktop/NodeJs/vueTurtorial/todo-list/webapi
  npx json-server --watch db.json

- ホストのサーバ立ち上げ
  cd /mnt/c/Users/xxx/Desktop/NodeJs/vueTurtorial/todo-list
  npm run serve
  http://localhost:8080/ にアクセス

# troubleshhting

1:1 error Parsing error: Unexpected token < -https://qiita.com/kurkuru/items/d4eebd34f0898c6a2d5a

エラー解除
