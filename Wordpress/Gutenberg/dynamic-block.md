PHPによる動的な生成を行うブロック。  
基本的には使用しないほうが望ましい。理由として  
- ブロックのプラグイン(creat-guten-block等)を無効にした場合、コンテンツごと消えてしまう。  
- ブロックが文法的に問題ない場合でも、PHP側のエラー等の原因で表示されなくなる場合がある。


## Reference 
https://capitalp.jp/2018/10/16/gutenberg-dynamic-block/  
https://github.com/WordPress/gutenberg/issues/4849#issuecomment-415566038
