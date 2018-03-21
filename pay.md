#支付API

```PHP 
在线支付
微擎中集成了目前主流的在线支付，分别如下：

微信支付 (https://pay.weixin.qq.com)
百度钱包 (http://b.baifubao.com)
银联支付 (http://mobile.unionpay.com/preference)
支付宝 (https://e.alipay.com/index.htm)
通过支付提供商申请到权限，在微擎中通过 功能选项 -> 支付参数 来开启某个支付方式。

微信支付需要设置支付授权域名 http://你的微擎域名/payment/wechat/ 和 http://你的微擎域名/app/


```

工作流程

```php
用户在使用模块功能需要支付时，模块调用父类的 $this->pay($params); 方法来调用系统支付功能。
系统收银台接到模块调用请求，生成支付界面（金额，商品信息等）。
用户在收银台中选择支付手段，如微信支付，支付宝支持等（需要在支付参数中设置开启）。
收银台根据用户选择的支付手段，请求到相应的支付接口上，用户完成支付。
完成支付后，系统会调用模块中的 $this->payResult($params); 方法来通知支付状态（成功或是失败）。

```

![支付流程](http://cdn.w7.cc/images/2017/08/02/15016129195980cb7730ddf_h7yd4YxC7o7O.jpg)