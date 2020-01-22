# marketplace-sdk-java

## marketplace方法说明

### 获取对象实例并设置marketplace-addon服务地址
```
getInstance(String restfulUrl)
```

### 初始化设置app域名和签名私钥
```
init(String domain, String wif)
```

### 设置marketplace-addon服务地址
```
setRestfulUrl(String restfulUrl)
```

### 生成上架数据的二维码参数
```
authOrder(String dataId, String symbol, String name, Integer amount, Long price, Integer transferCount, Integer accessCount,
                                Long expireTime, String makerReceiveAddress, String mpReceiveAddress, List<String> ojList)
```

### 生成下单购买的二维码参数
```
takeOrder(String authId,String takerReceiveAddress,Integer tokenAmount,String oj) throws Exception {
```

### 生成确认订单的二维码参数
```
confirmOrder(String orderId)
```

### 查询token信息
```
getTokenBalance(int tokenId)
```

### 查询二维码扫码结果
```
orderResult(String id)
```