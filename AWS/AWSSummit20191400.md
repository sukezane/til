#AWS Summit 2019 14:00-  
Amazon Managed Blockchain  

## Use Cases　
- ヘルスケア(カルテの改ざんを防ぐ)
- digital contents  

## related services  
### Blockchain partner  
### Blockchain template
- Cloudformation template  
#### QLDB  
- https://aws.amazon.com/jp/qldb/  
- 信頼される期間による中央集権型

### よくある質問  
#### 鍵管理のベストプラクティス  
- KMSで秘密鍵の管理  
- コンプライアンスの問題でハードウェア上で鍵を管理するなどの場合、Cloud HSMを使用する
  - CloudHSMの仕様例(Ginco)
  
## SME 事例  
### 音楽業界の課題  
- 中央管理団体で分配に関する情報が一部欠落しているため、欠落箇所を音楽出版社各社の独自DBで管理
- 検知登録や契約情報の確認などに人件費が発生→クリエイターへの還元の低下
- 権利処理を髪でやり取りするより、ブロックチェーンのほうがコストが安い
### Solution  
- Managed Blockchainでの台帳管理

### Architecture  
- 異なる法人間でmanaged blockchainのDBへのアクセスポイントを作成する  

