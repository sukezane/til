Vue.jsの基底コンポーネント(Dumb component)は以下のようなプレフィックスをつけた方が良い。  
```
BaseCard  
AppCard  
VCard
```
この考え方はReactの[Smart componentsとDumb components](https://medium.com/@thejasonfile/dumb-components-and-smart-components-e7b33a698d43)にも概念として存在する。  
Smart componentsはデータを持ち、状態の変化を司るコンポーネントである。(MVCで呼ぶところのコントローラーに近い）  
一方、Dumb componentsはそれ自体にデータは存在せず、表示のみを司るコンポーネントである。(MVCで呼ぶところのビューに近い)


## Reference  
https://jp.vuejs.org/v2/style-guide/index.html#%E5%9F%BA%E5%BA%95%E3%82%B3%E3%83%B3%E3%83%9D%E3%83%BC%E3%83%8D%E3%83%B3%E3%83%88%E3%81%AE%E5%90%8D%E5%89%8D-%E5%BC%B7%E3%81%8F%E6%8E%A8%E5%A5%A8  
https://medium.com/@sandoche/how-to-structure-a-vue-js-project-eabe75161882
