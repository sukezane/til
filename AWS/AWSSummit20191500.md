# EC2の進化の歴史から学ぶEC2入門  
- ハイパーバイザー型の仮想OS

## インスタンスタイプ編
- M1
  - vCPUに比例してメモリが大きくなるサイズが用意された
- C1
  - よりvCPUが大きいインスタンス
- M2
  - よりメモリサイズが大きいインスタンス
- cc1
  - 科学技術計算などクラスターコンピューティング用のインスタンス
- t1
  - 低負荷用のインスタンス
- cg1
  - GPU搭載のインスタンス
- cc2
  - cc1の後継インスタンス
- c5n
  - 最も広帯域なインスタンス
  - 最大100Gbps
  - レイテンシ10ms程度
- A1
  -スケール型ワークロードのコスト削減
  - ARMベースの開発環境
- f1
  - gpaを含んだインスタンス
  

  ### 採用技術
  最新のもの
 - Nitroベースの仮想化を採用
 - 内蔵ディスクをNVMeに
 
 #### Nitro
 #### ベアメタルインスタンス  
 - 仮想化されたインスタンでは利用できないワークロードに向けたインスタンス
 #### Needs
 商用ソフトウェアのライセンス対応
 ハイパーバイザーごと持ち込みたい  
 
 ## 機能編
 - ハードウェア専有インスタンスのユースケースは？
