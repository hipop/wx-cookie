# wx-cookie
重写微信小程序的wx.request，使之实现cookie的全部功能

### 工作目标

|目标|是否完成|
|:----|---:|
|解析response的http头部中的cookie信息  |  √ |
|将cookie存储到Storage中  |  √ |
|实现cookie的过期时间功能  | √ |
|实现cookie domain限制功能 | × |
|实现cookie path限制功能 | × |
|实现cookie httponly 限制功能 | × |
|提供js的cookie访问功能 | × |


### 使用方法
```javascript
// 引入
const cookieUtil = require("所在目录/wx-cookie.js");

// 发送请求
cookieUtil.request(OBJECT);
````
cookieUtil.request的使用方法完全兼容wx.request,
具体API，可参考微信官方文档[wx.request](https://developers.weixin.qq.com/miniprogram/dev/api/network-request.html#wxrequestobject)
