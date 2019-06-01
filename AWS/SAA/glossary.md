## 用語集  
### IPsec VPN  
IPsecと呼ばれる形式の専用回線  
https://wa3.i-3-i.info/word12038.html

### ハードウェアVPN  
オンプレミスとAWSサーバーの間をVPN接続する。  

### 仮想プライベートゲートウェイ  
オンプレミスとAWSサーバーを接続(ハードウェアVPN)する際にAWS側に設定するゲートウェイ。  
VPCのデフォルト設定ではVPC外のサーバーとの通信が確立できないため、これを使用して通信を行うよう設定できる。  
https://docs.aws.amazon.com/ja_jp/vpn/latest/s2svpn/VPC_VPN.html

### カスタマーゲートウェイ  
オンプレミスとAWSサーバーを接続(ハードウェアVPN)する際にユーザー側に設定するゲートウェイ。  

### インターフェイスVPCエンドポイント  
AWS PrivateLinkと同義。インターネットから出ることがなくサービス間をつなぐことができる。  
https://blog.mmmcorp.co.jp/blog/2017/11/15/aws_privatelink/  
https://docs.aws.amazon.com/ja_jp/vpc/latest/userguide/vpce-interface.html  

### ゲートウェイVPCエンドポイント  
ルートテーブルで使用するサービス（S3かDynamoDBが使用可能）を指定することでVPC外のサービスとつなげる。  
https://devlog.arksystems.co.jp/2018/05/11/4896/  

### ネットワークアーキテクチャ  
ネットワークアーキテクチャとは、ネットワークにおいて必要な論理構造やプロトコルを体系的に定めたもの。　　
代表的なアーキテクチャに、OSI参照モデルとTCP/IPモデルがある。  
http://bambinya.hateblo.jp/entry/2015/04/11/134458  

### オーバーヘッド  
ある処理に対して付加的に発生する処理のこと。  
https://wa3.i-3-i.info/word12471.html

### Egress-only インターネットゲートウェイ  
送信専用のインターネットゲートウェイのこと。Ipv6経由でインターネットに送信される。  
https://docs.aws.amazon.com/ja_jp/vpc/latest/userguide/egress-only-internet-gateway.html

### Network Load Balancer  
静的なIPをもつロードバランサー。毎秒数百万のリクエストを処理できる。
https://cloudpack.media/37201  
https://docs.aws.amazon.com/ja_jp/elasticloadbalancing/latest/network/introduction.html

### ワークロード  
稼働しているコンピューターのCPU使用率、メモリ使用率などの負荷の大きさ  
http://e-words.jp/w/%E3%83%AF%E3%83%BC%E3%82%AF%E3%83%AD%E3%83%BC%E3%83%89.html  
https://it-words.jp/w/E383AFE383BCE382AFE383ADE383BCE38389.html

### SWF  
https://aws.amazon.com/jp/swf/  
https://gist.github.com/gushernobindsme/f9694f55c892ee3f1ae7b83c187a488b#swf  

#### ワーカーとディサイダー  
https://aws.amazon.com/jp/swf/faqs/

### 仮想ネットワークインターフェース  
Elastic Network Interfaceのこと。  
仮想[NIC](https://wa3.i-3-i.info/word12498.html)の概念に近い。  
https://wa3.i-3-i.info/word12850.html

### Elastic Network Interface  
仮想ネットワークインターフェースのこと。  
ネットワークインターフェースの設定を保持しつつ他のインスタンスにアタッチすることができる。  

https://docs.aws.amazon.com/ja_jp/AWSEC2/latest/UserGuide/using-eni.html

### CIDR  
アドレス範囲を任意に設定する。
https://wa3.i-3-i.info/word11989.html

### Active Directory(AD)  
Windowsのサーバさんに搭載されている、ネットワークにつながっているパソコンとかをまとめて管理するための仕組み。  
あるドメイン内で認証済みのサーバーなどが互いに認証なしにやり取りできるようになる。  
https://wa3.i-3-i.info/word12420.html

### Simple AD  
Microsoft ADの機能が利用できる。
https://docs.aws.amazon.com/ja_jp/directoryservice/latest/admin-guide/directory_simple_ad.html

### トランザクション  
不可分な一連の処理のこと。
https://wa3.i-3-i.info/word142.html

### シーケンシャルアクセス（IO）  
ストレージへの連続的なアクセスのこと。  
HDDが得意とする。  
スループットが性能の指標として使われる。
https://cm.it-ex.com/c/focus/storage_iroha/index08.html

### ランダムアクセス（IO）  
ストレージへのランダムなアクセスのこと。  
SSDが得意とする。
IOPSが性能の修正として使われる。  
https://cm.it-ex.com/c/focus/storage_iroha/index08.html

### PV,HVM  
準仮想化、ハードウェア仮想化
https://qiita.com/namihitoo/items/e5201ac2c853b01c4975#hvmhardware-assited-vm

### ステートレス、ステートフル  
ステートレスは状態を維持し、ステートフルは状態に応じて変化が発生すること。
https://milestone-of-se.nesuke.com/nw-basic/as-nw-engineer/stateful-and-stateless/

### RDS(mysql)にSSL接続するコマンド  

```
mysql -h myinstance.c9akciq32.rds-us-east-1.amazonaws.com
--ssl-ca=[full path]rds-combined-ca-bundle.pem --ssl-mode=VERIFY_IDENTITY
```

## 参考  
https://5hintaro.com/it/aws-saa-fail/#st-toc-h-2  
