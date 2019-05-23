## ワイルドカードで複数指定できるが、一つ上のサブドメインレベルのみに限られる　　
例えば、example.comがZone Apexドメインであるとして、sub1.sub2.example.comの証明書を取得したい。  
その場合、*.sub2.example.comの証明書を発行することでsub1.sub2.example.comの証明書を発行できる。
http://blog.serverworks.co.jp/tech/2018/05/31/acm-wildcard-certificate/
