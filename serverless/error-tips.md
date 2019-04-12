## API Gateway
### Internal Server Errorが出る
- レスポンスの形式を以下のように指定しているか確認する
```
{
    "statusCode": httpStatusCode,
    "headers": { "headerName": "headerValue", ... },
    "body": "..."
}
```

https://qiita.com/_mogaming/items/4e9d8c62739399b076b7
https://forum.serverless.com/t/message-internal-server-error-on-api-gateway-responses-with-1-5/1117


## Cloudformation  
### スタックのアップデートに失敗する  
- DynamoDBのテーブル名を更新する  
https://forum.serverless.com/t/cloudformation-cannot-update-a-stack-when-a-custom-named-resource-requires-replacing/3217
