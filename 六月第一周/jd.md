# 药品信息详情展示功能小测试
## 1. Requirements
根据给出的图片参考和需求列表完成相应的功能
* 作为用户, 我需要通过输入用户名和密码验证并登录系统, 以便于以认证用户身份来使用药品展示平台
* 作为用户, 我需要有一个商品详情展示的页面, 这样以便于我可以得知一件药品的更多信息
## 2. To-Do listings
### 2.1 References
* ~~商品信息: 标题, 详情, 成都地区是否有货和支持配送的信息, 产品型号, 价格, 优惠获取价格, 一张商品图片~~

### 2.2 To-Do
* 根据列出的商品参考信息请设计数据库模型
* 根据需求搭建应用服务, 实现用户登录
* 实现登录用户浏览商品信息
  1. 从数据库获取商品标题, 详情, 图片(使用setTimeout延时1秒)
  2. 从数据库获取"成都"地区是否有货和支持配送的信息, 产品型号(使用setTimeout延时1秒)
  3. 获取基本价格, 优惠获取价格(使用setTimeout延时1秒)
  
* 加分设计: 访问以及渲染页面(页面加载时间<3s) 

