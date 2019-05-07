## 変数を含んだパスを別のものに入れ替えたい
変数パスを別のものに入れ替える場合、一度serverless.ymlから関数をコメントアウトしてからデプロイする。  
すると、API Gatewayの設定がリセットされるので、その後もう一度設定を戻してデプロイする。  
https://github.com/serverless/serverless/issues/3785#issuecomment-340784848
