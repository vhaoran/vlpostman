

host:       0755yicai.com
  登录方式：同im系统。

websocket:  0755yicai.com:8083/ws
 登录方式1： url方式
  测试登录： ws://0755yicai.com/ws?jwt=<jwtStr>
  eg :  ws://0755yicai.com:8083/ws?jwt=test|1
  其中，jwt的可以是以下方式： test|id .如：test|1表示id为1的jwt
登录方式2：header方式：
   测试：head["Jwt"] = test/<jwtStr>
   真实：ead["Jwt"] = <jwtStr> 
   
----登录-------------------------------   
系统中只有一个登录方法，适用于所有的角色。

   
  
            


