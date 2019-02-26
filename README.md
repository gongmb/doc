community 接口列表
==============

# 状态码


# 微信相关接口

##    1、名称:微信登录
        path:/weChat/getWxUserInfoByCode.json
        参数:
            参数类型		参数名				注释				必需
            String		    code				微信code			√

        返回值:
            {
                "userId": 2,
                "nickname": "Zoro",  //昵称
                "headimgurl": "http://thirdwx.qlogo.cn/mmopen/vi_32/DYAIOgq83erBCxkK9avxecCpTyibE1assI9Cib4ibV58TdKnhCjI9NDDIB4aWqFKe09v9aR0UPtvsgZjP6EjvqP9Q/132" //用户头像
            }

##     2、名称:微信分享
        path:/weChat/getWxShareInfo.json
        参数:
            参数类型		参数名				注释				必需
            String		    url				    分享路径			√

        返回值:
            {
                "code": "200",
                "msg": "成功",
                "data": {
                    "appid": "wx1455e6bc574303cd",
                    "noncestr": "founder2014",
                    "jsapi_ticket": "HoagFKDcsGMVCIY2vOjf9lf-gdMUV_n5aEQRY_FzpSJy7nJDc1kBt6viLQfG6afSm15FLE5JGIjQ3qrZDrBqlA",
                    "timestamp": "1523960073010",
                    "url": "http://handwriting.myfont.me/uploadWorks.html?activityId=1",
                    "signature": "9af68b4ad0c70e298d16a12f08c48097794136b5"
                }
            }



