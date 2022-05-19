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

- eslintrc.js を設定
  https://reffect.co.jp/vue/eslint#ESLint
- // eslint-disable-line で eslint を pass
  https://qiita.com/blajir/items/82127aaa57e4d73a8389

# Todo

追加ボタンが効かない。。。
->解決！
`store.vue`の以下の行が`http`なのに`https`になっていた！
await insertItems("https://localhost:3000/todos", data);
