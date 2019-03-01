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
            			"homeImage": "https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=2735633715,2749454924&fm=26&gp=0.jpg",
            			"previewImage": "https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=591147290,3111555510&fm=26&gp=0.jpg",
            			"actName": "活动名称0",
            			"remarks": "活动描述0",
            			"showStartTime": "2019-02-28T10:46:59.000+0000",
            			"showEndTime": "2019-03-05T10:46:59.000+0000",
            			"orderBy": 0,
            			"createDate": "2019-02-28T10:46:59.000+0000",
            			"createBy": "1111",
            			"updateDate": "2019-02-28T10:46:59.000+0000",
            			"updateBy": "1111",
            			"isDelete": "0",
            			"version": 1
            		}],
            		"genreList": [{ //类型列表
            			"id": "4a09edb576e04488a5528110be224c25",
            			"genreName": "测试类型0",
            			"nickname": "test_genre0",
            			"orderby": 0,
            			"createDate": "2019-02-28T10:43:28.000+0000",
            			"createBy": "1111",
            			"updateDate": "2019-02-28T10:43:28.000+0000",
            			"updateBy": "1111",
            			"isDelete": "0",
            			"version": 1
            		}],
            		"subjectList": [{ //主题列表
            			"id": "2444aab678a24f11a43e27f34b8a507e",
            			"subName": "测试主题0",
            			"nickname": "test_sub0",
            			"orderby": 0,
            			"createDate": "2019-02-28T10:46:56.000+0000",
            			"createBy": "1111",
            			"updateDate": "2019-02-28T10:46:56.000+0000",
            			"updateBy": "1111",
            			"isDelete": "0",
            			"version": 1
            		}]
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



