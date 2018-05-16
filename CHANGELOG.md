## 更新日志

### V 0.5.0
 
*2018-05-11*，项目支持微信支付和修复小程序的一些BUG
 
  * `小商场`因wx.getUserInfo接口调整，微信登录调整
  * `小商场`修复立即购买会下单购物车所有商品
  * `小商场`修复下单商品时添加收货地址成功但是没有显示
  * `小商场`修复下单商品时添加收货地址的地址信息不能滚动
  * `小商场`修复购物车商品不能删除
  * `小商场`支持微信支付
  * `管理后台`支持微信支付
  * `基础系统`数据库litemall_collect的id设置自增
  * `基础系统`数据库删除region相关的四个临时表
  * `基础系统`litemall-core模块swagger2配置，支持swagger文档
  * `项目`多模块maven结构重新设计
  * `项目`文档整理部署方案和上线方案
  * `项目`文档支持更新日志、贡献指南和常见问题

### V 0.4.0
 
*2018-04-21*，项目结构调整，增加了两个模块
 
  * `小商场`的后台服务代码添加注释，校验输入参数
  * `小商场`商品无货时显示“商品已售空”
  * `管理后台`支持管理员同一账户多终端登录，方便演示
  * `管理后台`专题内容支持富文本编辑
  * `基础系统`litemall-os-api的链接从`storage/index/index`调整至`os/index/index`
  * `基础系统`litemall-os-api支持浏览器显示。
  * `基础系统`新增litemall-core模块，综合了litemall-os-api、litemall-wx-api
     和litemall-admin-api的共性代码
  * `基础系统`新增litemall-all模块作为包裹模块，支持三个后台服务和静态文件
     打包成一个war项目包
     
### V 0.3.0 

*2018-04-07*，业务模块从物理删除调整成逻辑删除

* `小商场`的后台服务加密用户账号密码
* `小商场`如果用户选择货品，则显示货品对应的价格；否则显示商品价格
* `小商场`只有规格都选择，则商品页面才显示所对应货品的规格文本
* `管理后台`商品详细信息支持tinymce富文本编辑
* `管理后台`的后台服务加密管理员密码
* `管理后台`完善登录退出逻辑
* `基础系统`数据库中除regions几个表，其他所有表都添加`add_time`和`deleted`字段
* `基础系统`litemall-db模块不支持数据物理删除，删除则设置`deleted`，而查询则过滤`deleted`

### V 0.2.0

*2018-04-02*，修复一些小商场出现的问题。

* `小商场`微信登录
* `小商场`账号登录、注册、找回密码
  （注意手机验证码不支持，因此目前只是完成基本功能，但是存在安全风险）
* `小商场`订单编号采用日期+6位随机数
* `小商场`简单运费计算
* `小商场`专题评价
* `管理后台`禁止管理员修改超级管理员信息
* `基础系统`自动脚本util/lazy.sh和util/upload.sh
  
### V 0.1.0

*2018-03-24*， 项目架构基本完成。