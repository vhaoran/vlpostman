
master 3( uid,    )
broker_info 3  (ownere,id,name)
broker_admin 3 (bid/uid)
sys_admin 3
broker_master  3
user_info-->broker_info   3*3 broker的用户
broker_prize/vie_leveli --->   
broker-product



添加测试用户60个,id范围1-60, 密码默认为123456, 运营商, 大师,系统管理员分别10个,每个运营商添加3个运营商管理员(30个)

其中管理员UID范围为1-10 ------user_code(admin1~admin10)

大师uid范围为11-20  ------user_code(test_master1~test_master10), 每个大师开通两项业务,cate_id分别是1和2

运营商owner_id范围是21-30  -----user_code(test_broker1~test_broker10), 并且开启所有模块

运营商管理员UID范围是31-60  ----user_code(test_broker-admin1~test_broker-admin30),
	其中每个运营商下面有三个运营商管理员, 例如:
	owner_id为21的运营商,broker_id=1,其运营商管理员对应的UID分别为31, 41, 51 			  
	owner_id为22的运营商,broker_id=2,其运营商管理员对应的UID分别为32, 42, 52
运营商正式会员UID范围是61-80 ----user_code(test_user1-test_user20),
    其中为每个运营商添加两个非管理员的正式用户, 例如:
        owner_id=21的运营商,broker_id=1,其有两个非管理员的正式会员
            正式会员1:user_code=test_user1, uid=61 , broker_id=1
            正式会员2:user_code=test_user2, uid=62 , broker_id=1
运营商大师 为每一个运营商添加三个大师,大师的UID分别是11, 12, 13, 并为大师的项目添加价格,cate_id=1时 offset=100,cate_id=2时offset=200

运营商悬赏贴收费标准列表  为每个运营商添加三个平台悬赏贴收费标准 分别是1, 2, 3

运营商闪断贴收费标准列表  为每个运营商添加三个平台闪断贴收费标准 分别是1, 2, 3

运营商商品类别  为每个运营商选择已有的所有商品类别16, 17, 22, 30, 40, 41, 42, 43, 44, 45, 48, 50
  
运营商商品  为每个运营商添加2件商品,分别是:
        1:id_of_es="DHRGu3UBUEDNcUc8aIWj"---cate_id=48 
        2:d_of_es="D3RJu3UBUEDNcUc8oYVv"---cate_id=45 

测试数据示例:
       运营商: owner_id=21, user_code=test_broker1, id(broker_id)=1,
       运营商管理员:uid=31, user_code=test_broker-admin1, broker_id=1,
                   uid=41, user_code=test_broker-admin11, broker_id=1,
                   uid=51, user_code=test_broker-admin21, broker_id=1,
       正式会员(已经被代理的非运营商管理员用户):
                    uid=61, user_code=test_user1,broker_id=1,
                    uid=62, user_code=test_user2,broker_id=1,
       运营商大师: 
            大师1: broker_id=1,master_id=11,  
            大师2: broker_id=1,master_id=12, 
            大师3: broker_id=1,master_id=13, 
       运营商大师项目:
            项目1:broker_id=1, master_id=11,yi_cate_id=1, price_offset=200,
            项目2:broker_id=1, master_id=11,yi_cate_id=2, price_offset=200,
            项目3:broker_id=1, master_id=12,yi_cate_id=1, price_offset=200,
            项目4:broker_id=1, master_id=12,yi_cate_id=2, price_offset=200,
            项目5:broker_id=1, master_id=13,yi_cate_id=1, price_offset=200,
            项目6:broker_id=1, master_id=13,yi_cate_id=2, price_offset=200,
        运营商商品(默认已添加所有的商品种类):

