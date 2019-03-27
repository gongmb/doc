SSM-BOOK 接口列表
=============

# 状态码

# 首页
## 1、添加活码
        path:/ssm/book/addQr.json
        参数:
       {
            "arrayObj":[],//文件数组
            "activityName":"活动名称"
       }
        返回值:
        {
            "code": "200",
            "msg": "成功"
        }

## 2、更新活码
        path:/ssm/book/updateQr.json
        参数:
       {
            "arrayObj":[],//文件数组
            "id":1231 // ID
       }
        返回值:
        {
            "code": "200",
            "msg": "成功"
        }

## 3、活码列表
        path:/ssm/book/liveCodeList.json
        参数:
           {
            "current:":"1",
            "size":"1"
           }
        返回值:
        {
            "pageNum": 0,
            "pageSize": 1,
            "size": 1,
            "startRow": 1,
            "endRow": 1,
            "total": 21,
            "pages": 21,
            "list": [
                {
                    "id": 43,
                    "sourceContent": "http://test.tonglibang.com:12115/ssm/dispatch.html?o=91e349bd-25a9-44af-96de-2f41f9bca4f3",
                    "qrpath": "http://mallimghn.tonglibang.com/qr%2F%2F2019%2F3%2F22%2F3429ee67-6366-4237-adca-6f05cc00235d.gif?e=1553254167&token=Gx5UYQn_L_lmxekwJphwdcV-kNzKVC1wQfGjU5PY:FRZMJf0FhQbg0VNgaE_cXOy3ZNU=",
                    "uuid": "91e349bd-25a9-44af-96de-2f41f9bca4f3",
                    "activityName": "天津演示",
                    "createDate": "2019-03-22T10:29:26.000+0000"
                }
            ],
            "prePage": 0,
            "nextPage": 1,
            "isFirstPage": false,
            "isLastPage": false,
            "hasPreviousPage": false,
            "hasNextPage": true,
            "navigatePages": 8,
            "navigatepageNums": [
                1,
                2,
                3,
                4,
                5,
                6,
                7,
                8
            ],
            "navigateFirstPage": 1,
            "navigateLastPage": 8,
            "firstPage": 1,
            "lastPage": 8
        }

