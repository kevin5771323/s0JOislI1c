# 前言

微信点餐系统小程序是基于SSM框架和微信小程序平台开发的便捷的点餐工具。该项目旨在帮助商家简化点餐流程，提高工作效率，同时也为顾客提供更优质的点餐体验。

# 内容介绍

本项目主要包括以下功能模块：菜品展示、菜品分类、购物车、订单管理、用户管理等。用户可以通过微信小程序方便地浏览菜品、添加购物车、提交订单，并实时查看订单状态。商家可以在后台管理系统中进行菜品管理、订单处理等操作。

# 技术介绍

## 语言：Java

## 使用框架：Spring Springmvc，MyBatis，微信小程序

## 前端技术：JS、Vue、CSS3，Uniapp

## 开发工具：IDEA/Eclipse，Uniapp

## 数据库：MySQL 5.7/8.0

## 数据库管理工具：phpStudy/Navicat

## JDK版本：jdk1.8

## Maven：apache-maven 3.8.1-bin

## 前端环境：Node.Js 12\14\16

# 核心代码

以下为购物车模块的部分核心代码：

```java
@Service
public class ShoppingCartService {

    @Autowired
    private ShoppingCartMapper shoppingCartMapper;

    // 添加商品到购物车
    public int addGoodsToCart(ShoppingCart cart) {
        return shoppingCartMapper.insert(cart);
    }

    // 修改购物车商品数量
    public int updateCartGoodsCount(Integer id, Integer goodsCount) {
        ShoppingCart cart = new ShoppingCart();
        cart.setId(id);
        cart.setGoodsCount(goodsCount);
        return shoppingCartMapper.updateByPrimaryKeySelective(cart);
    }

    // 查询购物车列表
    public List<ShoppingCart> getCartListByUserId(Integer userId) {
        return shoppingCartMapper.selectByUserId(userId);
    }
}
```

# 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图
![封面图片](https://img11.360buyimg.com/ddimg/jfs/t1/350980/3/3016/188547/68c5a274Fbd60910b/bc616651cb988194.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/326891/29/19667/39466/68c5a24bF51e18fcd/f58f17fbb87ca6d8.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/332321/34/13116/100769/68c5a24cF62e71761/2b17766260c0fdf9.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/351194/39/3097/100334/68c5a24cF57353eef/4afffee65196dcb6.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/330663/35/12956/68929/68c5a24dFf2630b69/e4b5c1f996394b1a.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/340556/18/10487/22555/68c5a24dF8ba08ff2/34218436bf477483.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/323651/39/19848/74686/68c5a24dF5983221b/225dcde1ae5fe76e.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/332651/33/12803/15790/68c5a24dF5ddec321/9a675e4bf588dfc2.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/341706/31/3112/129059/68c5a24dFc134f938/3d5a87d7f593931a.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/346648/10/3026/13854/68c5a24dF8f258335/86b67feffb42fd50.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
