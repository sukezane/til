# Ch.5  
## 5.1  
- 動的コンポーネント  
https://jp.vuejs.org/v2/guide/components.html#%E5%8B%95%E7%9A%84%E3%81%AA%E3%82%B3%E3%83%B3%E3%83%9D%E3%83%BC%E3%83%8D%E3%83%B3%E3%83%88
https://jp.vuejs.org/v2/guide/components-dynamic-async.html  

補足
状態のトランジション
- アニメーションはDOMの変更にのみ適用される
- データの状態に対してアニメーションをしたい場合、$watchで監視する

# 5.2
- slotがルートエレメントに定義できない理由
https://stackoverflow.com/questions/49046697/vue-root-element-content-and-content-distribution-slots  

- slot-scopeでv-ifを使用できない理由

# 5.3  
カスタムディレクティブ
- updateフックは関係ないデータの変更に対して検知しないように処理する必要がある
  - img-fallbackでsrcの内容に変更がない場合でも、alt属性に変更があった場合にupdateフックが作動してしまうため  

### 5.3.2  
#### VNode  
- どのノードを描画するかを記述した情報。仮想DOMはこの総体
https://jp.vuejs.org/v2/guide/render-function.html#%E4%BB%AE%E6%83%B3-DOM

# 5.4  
- mixinアンチパターン  
https://aloerina01.github.io/blog/2018-12-25-1
- mixinのユースケースは？
