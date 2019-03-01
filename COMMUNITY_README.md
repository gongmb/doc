community 接口列表
==============

# 状态码

# 首页
## 1、获取首页信息
        path:/community/subject/getIndexInfo.json
        参数:
        参数类型		参数名				注释				必需

        返回值:
            {
            	"code": "200",
            	"msg": "成功",
            	"data": {
            		"activityList": [{ //活动列表
            			 "id": "cd9976ebe98e40678cb9149576b0d8bc",
                        "homeImage": "https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=2735633715,2749454924&fm=26&gp=0.jpg"
            		}],
            		"genreList": [{ //类型列表
            			   "id": "a6f7dac2784f41a48e80e2d27fe56c4c",
                            "genreName": "测试类型-一级类型0",
                            "headimage": "http://pic33.photophoto.cn/20141114/0005018350653217_b.jpg"
            		}],
            		"subjectList": [{ //主题列表
            			 "id": "d656afde1c14496c80b24b445f41a810",
                        "subName": "测试主题0"
            		}]
            	}
            }
## 2、根据上级ID查询类型列表
        path:/community/genre/getGenreListParentId.json
        参数:
            {
                "parentId":"a6f7dac2784f41a48e80e2d27fe56c4c"
            }
        返回值:
            {
                "code": "200",
                "msg": "成功",
                "data": [
                    {
                        "id": "1ad4bad011304c729b32b85a6a56ec10",
                        "mainTitle": "主标题0",
                        "subtitle": "副标题0",
                        "headimage": "http://pic33.photophoto.cn/20141230/0005018362196390_b.jpg"
                    },
                    {
                        "id": "40831c241f6a4f74bc7b3ecf9cf21c19",
                        "mainTitle": "主标题0",
                        "subtitle": "副标题0",
                        "headimage": "http://pic33.photophoto.cn/20141230/0005018362196390_b.jpg"
                    },
                    {
                        "id": "60cee8fae76b4744bcecd5ccaf4b5fc4",
                        "mainTitle": "主标题0",
                        "subtitle": "副标题0",
                        "headimage": "http://pic33.photophoto.cn/20141230/0005018362196390_b.jpg"
                    },
                    {
                        "id": "750b841a7cf848fdbc151ba9a255e740",
                        "mainTitle": "主标题0",
                        "subtitle": "副标题0",
                        "headimage": "http://pic33.photophoto.cn/20141230/0005018362196390_b.jpg"
                    },
                    {
                        "id": "eb4e1d89e8964f02bb2e6c7979197b2d",
                        "mainTitle": "主标题0",
                        "subtitle": "副标题0",
                        "headimage": "http://pic33.photophoto.cn/20141230/0005018362196390_b.jpg"
                    }
                ]
            }
## 3、查询社群列表
        path:/community/communityInfo/getCommunityInfoList.json
        参数:
        {
        	 "current":"1",
              "size":"1"
        }

        返回值:
            {
                "code": "200",
                "msg": "成功",
                "data": {
                    "current": 1,
                    "size": 1,
                    "total": 100,
                    "haveNextPage": true,
                    "communityResultBoList": [
                        {
                            "mainTitle": "主标题99",
                            "subTitle": "副标题99",
                            "headImage": "http://img.pconline.com.cn/images/upload/upc/tx/photoblog/1405/31/c0/34808184_34808184_1401494219156_mthumb.jpg",
                            "id": "d9185780d6fe408792a9cf1c1be9fe46"
                        }
                    ]
                }
            }

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



