# AWS Summit 2019
## 11:00- 

### AWS SAM
- Cloudformation拡張
- Seeverless Frameworkみたいなもの

### ローカル開発
- step functions local
- dynamodb local
- local stack  

###　セキュリティとガバナンス  
#### Secutiry
- function policy  
- execution role  

#### Govvernance  
- Cloud Trail
  - data event
    - 読み出しのリクエストなどをすべて記録
    
- AWS Config
  - AWSリソースの監視
  - ポリシーが構成に準拠しているかを監#
#### Lambda Layer  
- あらゆるファンクションからコードを共有できるライブラリみたいな
- bersioning
- その他のアカウントとも共有可能

### Monitoring/Logging/Troubleshoot
#### Cloudwatch
- 
#### X-Ray
profiling, troubleshoot  
- lambdaのすべての言語に台うすrいリクエストのフローを記録
- X-Ray Analyticsで時系列ごとにリクエストのデバッグが可能

#### Lambda仕様
CPUコアとメモリ幼鳥の割合は比例して割り当てられる　　
メモリを上げたからといってコストがそれに比例して上昇するわけではない

#### how to iinvestigate
- debu:in <function>での cloudwatch Log出力

