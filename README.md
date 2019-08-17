[TOC]

# 开放平台自建应用接入 Demo

## 配置文件说明
> application.properties

配置文件配置好自建应用的相应参数

```
# 自建应用KEY
app.key=<your App Key>

# 自建应用SECRET
app.secret=<your Secret>

# 自建应用appcode
app.code=<your App Code >
```

## 常用地址
[友空间门户](https://ec.diwork.com/portal/home/index#/)

[友空间文档中心](https://open.diwork.com/#/prodService/applyOpen/uspace)

[diwork工作台](https://www.diwork.com/#/)

[用友云开放平台](https://open.diwork.com/#/)

## 根据code免登demo

地址：{serverUrl}/freelogin_view

可通过服务端REST (com.yonyou.iuap.corp.demo.web.FreeLoginDemoController.getFreeLoginInfo）, 打开页面templates/freelogin_view.html

## jsbridge demo

地址：{serverUrl}/jsdemo

可通过服务端REST（com.yonyou.iuap.corp.demo.web.JsBridgeDemoController.jsdemo）, 打开页面templates/index.html

## 自建应用接入文档参见文档中心
[自建应用接入](https://open.diwork.com/#/docs/md2docs/open-api-doc?id=xietong&section=3).

## 常用API接口
> 接口文档可参见 [服务端API](https://open.diwork.com/#/docs/md2docs/open-api-doc?id=xietong&section=16)

- 获取自建应用access_token

  代码参考 com.yonyou.iuap.corp.demo.web.ApiController.getAccessToken

- 获取jsticket

  代码参考 com.yonyou.iuap.corp.demo.web.ApiController.getJsticket

- 生成jsapi鉴权信息

  代码参考 com.yonyou.iuap.corp.demo.web.ApiController.getAgentInfo

- 根据code获取免登信息

  代码参考 com.yonyou.iuap.corp.demo.web.ApiController.getFreeLoginInfo

- 分页查询用户信息

  代码参考 com.yonyou.iuap.corp.demo.web.ApiController.getUserPageList

- 根据用户ids查询用户信息

  代码参考 com.yonyou.iuap.corp.demo.web.ApiController.getUserListByIds

- 根据 手机号/邮箱/用户名 搜索用户

  代码参考 com.yonyou.iuap.corp.demo.web.ApiController.searchUser

- 分页查询当前租户员工列表

  代码参考 com.yonyou.iuap.corp.demo.web.ApiController.getStaffPageList

- 根据手机号或则邮箱查询当前租户员工列表

  代码参考 com.yonyou.iuap.corp.demo.web.ApiController.searchStaffByMobileOrEmail

- 发送工作通知

  代码参考 com.yonyou.iuap.corp.demo.web.ApiController.sendNotifyShare

- 发送待办事件

  代码参考 com.yonyou.iuap.corp.demo.web.ApiController.sendToDo

- 标记待办事件为已处理

  代码参考 com.yonyou.iuap.corp.demo.web.ApiController.sendDone

- 删除待办事件

  代码参考 com.yonyou.iuap.corp.demo.web.ApiController.revocation