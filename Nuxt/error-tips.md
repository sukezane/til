# asyncDataにaxiosでServerMiddlewareからデータを取得するURLを書いてNetlifyにデプロイしたら"Request failed with status code 404"と出てページにアクセスできなくなる
## 前提  
- プロダクション環境
- serverMiddlewareはaxiosで自己のドメインのAPIにアクセスする
## 原因
Netlifyでプロダクションビルドでデプロイした場合、一度nuxtで起動していたサイトをオフにしてから'nuxt generate'をしているため、自己のドメインに対してのアクセスができなくなり、"Request failed with status code 404"と表示されてしまう。  
## 対処法  
asyncDataに記述せず、クライアント側の方でデータを取得するようにすると動いた。
