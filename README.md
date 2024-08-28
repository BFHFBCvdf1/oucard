<p align="center"><img src="https://s2.loli.net/2024/05/09/zFKnq6LASRh3boa.png" width="200"></p>

<p align="center">
<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/license-MIT-blue" alt="license MIT"></a>
<a href="https://github.com/assimon/dujiaoka/releases/tag/2.0.6.01"><img src="https://img.shields.io/badge/version-2.0.6.01-red" alt="version 2.0.4"></a>
<a href="https://www.php.net/releases/7_4_0.php"><img src="https://img.shields.io/badge/PHP-7.4-lightgrey" alt="php74"></a>
<a href="https://t.me/+v16BXiiwU4U5ZjEx"><img src="https://img.shields.io/badge/TG群-OU社区-green" alt="TG群:https://t.me/+v16BXiiwU4U5ZjEx"></a>
<a href="https://t.me/buzhiguiqi"><img src="https://img.shields.io/badge/TG客服-buzhiguiqi-green" alt="TG群:https://t.me/buzhiguiqi"></a>
</p>

### 发卡机器人多语言介绍

TG自动/自助发卡机器人/USDT发卡机器人/多语言发卡机器人/带web后台/独角发卡机器人,基于独角数卡魔改完成,集成epusdt支付,相比上一版本新增了安全增强的功能，但不排除没有漏洞和bug，使用了telegram-bot/api作为机器人第三方类库，开发环境phpstorm+php7.4+mysql5.7+redis进行开发，可对其进行二次开发!

# 发卡机器人多语言版功能介绍

* 新增机器人多语言选择(可销售至国外任何国家)

* 后台自定义添加语言种类(可自定义语言数量)

* 安全增强,对其用户发送的内容做了过滤处理,更安全更可靠

* 增加发卡种类,纯文本卡密,文件卡密,URL卡密(不再是单一的发卡)

* 所有的按钮以及展示文字都写在了语言包(只需要新增语言包和修改语言包即可完成机器人的装修)

* 增强后台认证

* 后台可自定义开关订单确认页面

* 取消了按钮自定义输入数量，在商品页面可直接输入数量即可实现购买数量

* 模块化开发，每一个按钮都是一个类，加密授权后也可进行二次开发

* 新增统计推广人数以及推广佣金统计。

### 使用交流

Telegram交流更新群: https://t.me/openfaka
客服:https://t.me/buzhiguiqi

# 推荐服务器和域名
- （digitalocean数字海洋，优先选择加拿大多伦多2核2G）[👉🏻点我直达](https://cloud.digitalocean.com/)
- （gname域名可USDT支付）[👉🏻点我直达](https://www.gname.com/)

## 界面展示
【后台首页展示】
![home.png](https://s2.loli.net/2024/05/09/Fhcg58NedD3aj7t.png)

【英语版商品列表展示】
![ 2024-05-09 153236.png](https://s2.loli.net/2024/05/09/Sh948BXPLM1VIuR.png)

【英语版商品不带图片详情展示】
![ 2024-05-09 153304.png](https://s2.loli.net/2024/05/09/gQSGCua58ZiyLAF.png)

【英语版商品带图片详情展示】
![ 2024-05-09 153333.png](https://s2.loli.net/2024/05/09/gZVpBfAKwDsxUzF.png)

【中文版商品带图片详情展示】
![ 2024-05-09 154351.png](https://s2.loli.net/2024/05/09/LUlGg9DxBd2e3Ac.png)

## 安装篇
- [Linux环境安装](https://github.com/assimon/dujiaoka/wiki/linux_install)
- [Docker安装](https://github.com/assimon/dujiaoka/wiki/docker_install)
- [2.x版本宝塔安装教程](https://github.com/assimon/dujiaoka/wiki/2.x_bt_install)
- [1.x版本宝塔环境安装](https://github.com/assimon/dujiaoka/wiki/1.x_bt_install)
- [常见问题锦集-你遇到的问题大部分能在这里找到解决！！](https://github.com/assimon/dujiaoka/wiki/problems)
- [系统升级](https://github.com/assimon/dujiaoka/wiki/update)
- [各支付对应后台配置](https://github.com/assimon/dujiaoka/wiki/problems#各支付对应配置)
- [视频教程及工具集合](https://pan.dujiaoka.com)

## 支付接口已集成
- [x] 支付宝当面付
- [x] 支付宝PC支付
- [x] 支付宝手机支付
- [x] [payjs微信扫码](http://payjs.cn).
- [x] [Paysapi(支付宝/微信)](https://www.paysapi.com/).
- [x] 码支付(QQ/支付宝/微信)
- [x] 微信企业扫码支付
- [x] [Paypal支付(默认美元)](https://www.paypal.com)
- [x] V免签支付
- [x] 全网易支付支持(通用彩虹版)
- [x] [stripe](https://stripe.com/)
- [x] [EPUSDT](https://github.com/assimon/epusdt)(已支持)
- [x] 余额支付(已支持)

## 基本环境要求

- (PHP + PHPCLI) version = 7.4
- Nginx version >= 1.16
- MYSQL version >= 5.6
- Redis (高性能缓存服务)
- Supervisor (一个python编写的进程管理服务)
- Composer (PHP包管理器)
- Linux (Win下未测试，建议直接Linux)
- /public/session + /public/txt 必须拥有777权限

## PHP环境要求

星号(*)为必须执行的要求，其他为建议内容

- **\*安装`fileinfo`扩展**
- **\*安装`redis`扩展**
- **\*安装`swoole_loader`扩展**
- **\*终端需支持`php-cli`，测试`php -v`(版本必须一致)**
- **\*需要开启的函数：`putenv`，`proc_open`，`pcntl_signal`，`pcntl_alarm`**
- 安装`opcache`扩展

## 演示及默认后台

- 演示后台: https://caonima.cl.kime.eu.org/admin    用户名:admin  密码:admin
- 演示机器人: https://t.me/testkaifaBot
- 演示站为1核1G的服务器,测试起来相对比较卡

- 后台路径 `/admin`
- 默认管理员账号 `admin`
- 默认管理员密码 `admin`

## 免责声明

该程序是未独角二次开发产品，仅用于学习交流使用！       
不可用于任何违反**中华人民共和(含台湾省)**或**使用者所在地区**法律法规的用途。      
因为本人仅完成代码的二次开发，从未参与用户的任何运营和盈利活动。    
且不知晓用户后续将**程序源代码**用于何种用途，故用户使用过程中所带来的任何法律责任即由用户自己承担。   
本系统不得用于**黄毒赌CVV电子烟国内实名账号**等违法内容

## 售价
此版本售价75U提供搭建图文教程搭建视频教程
150U提供一次搭建服务和迁移服务在75U基础上增加一年更新服务
350U在150U的基础上增加1年的技术支持
永久收款地址:`TD1iCRED5x9rbDDrR8fJzKpcxfkr4rYioU`

## 免费版本使用
目前市面上正在销售的独角发卡机器人都是从这里流出去被破解的，他们所卖的系统均为盗版，且本人已提供免费下载并使用的下载链接，在群里和论坛均可找到，其他人卖的均为骗子或盗版<br/>已知的盗版有:https://github.com/cnmbdb/HF-dujiao-faka-tg_bot