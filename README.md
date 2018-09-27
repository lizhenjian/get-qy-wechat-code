# get-qy-wechat-code
绕开企业微信可信域名，授权域名只能填写一个

使用样例 将html文件放置到可信域名可访问目录
```
$redirectUrl =  urlencode('http://'.$_SERVER['SERVER_NAME'].$_SERVER["REQUEST_URI"]);
$Url = 'http://XXX.com/get-code.html?appid=appid&redirect_uri='.$redirectUrl.'&response_type=code&scope=snsapi_userinfo&state=STATE#wechat_redirect';
redirect($Url);
```
