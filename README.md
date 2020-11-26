# vlpostman



每个微服务一个postman文件

mkdir yi
yicms.postman


添加测试用户60个,id范围1-60(user_info中前十条), 密码默认为123456, 运营商, 大师,系统管理员分别10个,每个运营商添加3个运营商管理员(30)

其中管理员UID范围为1-10, id范围是1-10------user_code(admin1~admin10)

大师uid范围为11-20, id范围是1-10------user_code(test_master1~test_master10), 每个大师开通两项业务,cate_id分别是1和2

运营商owner_id范围是21-30, id范围是1-10-----user_code(test_broker1~test_broker10), 并且开启所有模块

运营商管理员UID范围是31-60, id范围是1-30----user_code(test_broker-admin1~test_broker-admin10),
	其中每个运营商下面有三个运营商管理员, 例如:
	owner_id为21的运营商,broker_id=1,其运营商管理员对应的UID分别为31, 41, 51 			  
	owner_id为22的运营商,broker_id=2,其运营商管理员对应的UID分别为32, 42, 52
运营商大师 为每一个运营商添加三个大师,大师的UID分别是11, 12, 13, 并为大师的项目添加价格,cate_id=1时offset=100,cate_id=2时offset=200

运营商悬赏贴收费标准列表  为每个运营商添加三个平台悬赏贴收费标准 分别是1, 2, 3

运营商闪断贴收费标准列表  为每个运营商添加三个平台闪断贴收费标准 分别是1, 2, 3

运营商商品类别  为每个运营商选择已有的所有商品类别16, 17, 22, 30, 40, 41, 42, 43, 44, 45, 48, 50
  
运营商商品  为每个运营商添加三件商品,分别是:
        1:id_of_es="BnT7aHUBUEDNcUc8y4Ue0"---cate_id=16 
        2:id_of_es="DHRGu3UBUEDNcUc8aIWj"---cate_id=48 
        1:id_of_es="D3RJu3UBUEDNcUc8oYVv"---cate_id=45 




