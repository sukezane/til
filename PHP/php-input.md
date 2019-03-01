# php inputとは  
リクエストボディを直接参照できる。 `php://input`  

# $_POSTとの違い  
- php.iniの`max_input_vars`に依存しないため、大量のデータを扱う際に向く。
- enctype=”multipart/form-data” に対しては使用できない

## Reference  
http://ivystar.jp/programming/php/what-is-phpinput/
