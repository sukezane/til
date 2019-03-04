ajaxでbooleanの値を送信した場合、Stringとして値が送信されるため、falseの値を送ってもtrueと判定されてしまう。
一方、fetchでは値をそのまま受け取るため、booleanのままで値が送信される。

## Reference  
http://absg.hatenablog.com/entry/2016/03/21/181310
