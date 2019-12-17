# asyncDataにaxiosでServerMiddlewareからデータを取得するURLを書いてNetlifyにデプロイしたら"Request failed with status code 404"と出てページにアクセスできなくなる
## 前提  
- プロダクション環境
- serverMiddlewareはaxiosで自己のドメインのAPIにアクセスする
## 原因
Netlifyでプロダクションビルドでデプロイした場合、一度サーバー
