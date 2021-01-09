# 测试数据
## 测试用户:
    添加测试用户80个,id范围1-80, 密码默认为123456, 其中运营商, 大师,系统管理员分别10个,每个运营商添加3个运营商管理员(共30个), 每个运营商添加2个正式用户(共20个)  

## 系统管理员:  
    UID范围为1-10 ------user_code(admin1~admin10)  

## 大师:  
    uid范围为11-20  ------user_code(master1~master10), 每个大师开通两项业务,cate_id分别是1和2  

## 运营商:  
    owner_id范围是21-30  -----user_code(broker1~broker10), 并且开启所有模块  

## 运营商管理员:  
    UID范围是31-60  ----user_code(badmin1~badmin30)  
	其中每个运营商下面有三个运营商管理员, 例如:
	    owner_id为21的运营商,broker_id=1,其运营商管理员对应的UID分别为31, 41, 51 	
	    owner_id为22的运营商,broker_id=2,其运营商管理员对应的UID分别为32, 42, 52

## 运营商正式会员:  
    UID范围是61-80 ----user_code(user1~user20)    
    其中为每个运营商添加两个非管理员的正式用户, 例如:  
    owner_id=21的运营商,broker_id=1,其有两个非管理员的正式会员  
            正式会员1:user_code=user1, uid=61 , broker_id=1  
            正式会员2:user_code=user2, uid=62 , broker_id=1  
## 运营商大师:  
    为每一个运营商添加三个大师,大师的UID分别是11, 12, 13, 并为大师的项目添加价格,cate_id=1时 offset=100,cate_id=2时offset=200  

## 运营商悬赏贴收费标准列表:  
    为每个运营商添加三个平台悬赏贴收费标准 分别是1, 2, 3

## 运营商闪断贴收费标准列表:  
    为每个运营商添加三个平台闪断贴收费标准 分别是1, 2, 3

## 运营商商品类别:  
    为每个运营商选择已有的所有商品类别17, 30, 40, 41, 42, 43, 45
  
## 运营商商品:  
    为每个运营商添加1件商品,分别是:
        1:d_of_es="D3RJu3UBUEDNcUc8oYVv"---cate_id=45 

# 测试数据示例:  
       运营商: owner_id=21, user_code=broker1, id(broker_id)=1  
       运营商管理员:uid=31, user_code=badmin1, broker_id=1  
                   uid=41, user_code=badmin11, broker_id=1  
                   uid=51, user_code=badmin21, broker_id=1  
       正式会员(已经被代理的非运营商管理员用户):  
                    uid=61, user_code=user1,broker_id=1,  
                    uid=62, user_code=user2,broker_id=1,  
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
        运营商商品(默认已添加所有的商品种类)  
        系统管理员:   
            user_code=admin1, uid=1  
        大师:   
            user_code=master1, uid=11  
         

