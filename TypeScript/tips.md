## オブジェクトのプロパティを動的に追加する  
ajaxなどで返ってくるレスポンスの型が複数存在したり、レスポンス内容が将来的に変更される可能性がある場合、`var obj: {[k: string]: any} = {};`のように定義する。  
https://stackoverflow.com/questions/12710905/how-do-i-dynamically-assign-properties-to-an-object-in-typescript

## オブジェクトの定義の仕方  
https://qiita.com/nogson/items/63519abe945cfa806951#%E5%A4%89%E6%95%B0%E3%81%AB%E3%82%AA%E3%83%96%E3%82%B8%E3%82%A7%E3%82%AF%E3%83%88%E3%82%92%E5%85%A5%E3%82%8C%E3%82%8B%E5%A0%B4%E5%90%88%E3%81%AE%E5%9E%8B%E5%AE%9A%E7%BE%A9%E6%96%B9%E6%B3%95

## 外部の関数を参照する  
外部の関数を参照する場合、関数を変数に入れ`declare const functionName: any;`の形式でvue.shims.d.tsファイルに変数を宣言する。
