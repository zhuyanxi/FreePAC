美国 VPS [Hostwinds](https://affiliates.hostwinds.com/hostwinds.php?id=7011&url=1224) 是一款非常不错的 VPS，Hostwinds 搭建 SSR 是不错的选择，今天就讲解下 Hostwinds 搭建 SSR 教程。

## 1、购买 Hostwinds VPS

首先确认不要使用任何代理，网络是什么 IP 就是什么 IP ，不然可能需要人工审核，导致 Hostwinds VPS 购买显示 "Pending" 状态， 不能即时创建服务激活。

1、通过[ Hostwinds 优惠链接进入](https://affiliates.hostwinds.com/hostwinds.php?id=7011&url=1224)Hostwinds 首页，选择 “VPS” 下的 "Unmanaged VPS" ，这里是最便宜的**(注意千万不要选择页面上 3.29 美元那个，那个是虚拟空间，不是 VPS !!!)**。

[![img](https://user-images.githubusercontent.com/52620310/62405902-216e0d00-b5d6-11e9-8361-a3a75797b52f.jpg)](https://user-images.githubusercontent.com/52620310/62405902-216e0d00-b5d6-11e9-8361-a3a75797b52f.jpg)

2、进入 VPS 选择页面后，根据自己的需要的配置选择套餐，一般我们选择最低配置就够用了，然后点击 “Order” 按钮进入信息填写页面，如下所示：

[![img](https://user-images.githubusercontent.com/52620310/62405905-27fc8480-b5d6-11e9-85d3-70c4f202ef17.jpg)](https://user-images.githubusercontent.com/52620310/62405905-27fc8480-b5d6-11e9-85d3-70c4f202ef17.jpg)

3、进入信息填写页面后首先填写账号信息，一般是新用户我们填写左边的姓、名、邮箱、密码，然后点击 “Submit” 进入下一步，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405907-2cc13880-b5d6-11e9-8dd3-bca5e119f97d.jpg)](https://user-images.githubusercontent.com/52620310/62405907-2cc13880-b5d6-11e9-8dd3-bca5e119f97d.jpg)

4、页面跳转后填写用户信息，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405909-321e8300-b5d6-11e9-8efc-d25563e38ea1.jpg)](https://user-images.githubusercontent.com/52620310/62405909-321e8300-b5d6-11e9-8efc-d25563e38ea1.jpg)

5、然后选择购买时间、数据中心 、操作系统，红色部分需要自己选择，绿色一般我们默认，可以按月购买，但是建议第一次购买时间选择长一点，这样优惠要大很多，不然后面续费优惠力度就没有这么大了。 如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405910-36e33700-b5d6-11e9-916a-21611cae95ba.jpg)](https://user-images.githubusercontent.com/52620310/62405910-36e33700-b5d6-11e9-916a-21611cae95ba.jpg)

6、默认是自动云备份的，如果不需要去掉勾选， 如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405913-3c408180-b5d6-11e9-908d-d475887eda70.jpg)](https://user-images.githubusercontent.com/52620310/62405913-3c408180-b5d6-11e9-908d-d475887eda70.jpg)

7、然后选择付款方式，一般我们选择支付宝进行付款 （只有国内 IP 访问的时候才有支付宝付款方式），如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405915-406c9f00-b5d6-11e9-90d8-7eed10538637.jpg)](https://user-images.githubusercontent.com/52620310/62405915-406c9f00-b5d6-11e9-90d8-7eed10538637.jpg)

8、最后确认价格（不同时期可能价格有些许不同，如果通过前面优惠链接点击购买会有优惠），勾选同意协议，然后点击“Complete Order”按钮进行下单， 如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405916-4498bc80-b5d6-11e9-8ecd-77d1f9587e94.jpg)](https://user-images.githubusercontent.com/52620310/62405916-4498bc80-b5d6-11e9-8ecd-77d1f9587e94.jpg)

9、下单完成后订单结果如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405918-482c4380-b5d6-11e9-970d-4fce99d5d1e6.jpg)](https://user-images.githubusercontent.com/52620310/62405918-482c4380-b5d6-11e9-970d-4fce99d5d1e6.jpg)

## 2、SSH 连接 Hostwinds

首先你需要通过 SSH 连接 [Hostwinds](https://affiliates.hostwinds.com/hostwinds.php?id=7011&url=1216) 的 Linux VPS，连接 Linux VPS 需要使用 SSH 工具，这里推荐使用 Xshell 可以复制粘贴命令，Xshell 本身是需要付款的，作为中国人当然是使用 XX 版了，这里提供下载包如下所示：

Xshell 下载地址：<https://pan.baidu.com/s/1v7RCM0IjZGn_q5aWS1WXWg>，提取码: q3jw

下载后解压安装即可。

#### 使用 Xshell 连接 Linux VPS

1、打开 Xshell，点击左上角“文件”-“新建”，打开连接弹出库。

[![img](https://user-images.githubusercontent.com/52620310/62405920-537f6f00-b5d6-11e9-8665-b9ff1741d477.jpg)](https://user-images.githubusercontent.com/52620310/62405920-537f6f00-b5d6-11e9-8665-b9ff1741d477.jpg)

2、在 Xshell 弹出框中输入 IP 和端口，端口一般是 22 默认，然后点击确认按钮，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405922-567a5f80-b5d6-11e9-8b7a-2662799e0585.jpg)](https://user-images.githubusercontent.com/52620310/62405922-567a5f80-b5d6-11e9-8b7a-2662799e0585.jpg)

3、然后输入用户名 root，勾选记住用户名。

[![img](https://user-images.githubusercontent.com/52620310/62405925-5a0de680-b5d6-11e9-87bf-426f33dab264.jpg)](https://user-images.githubusercontent.com/52620310/62405925-5a0de680-b5d6-11e9-87bf-426f33dab264.jpg)

4、然后输入密码，勾选记住密码，点击确定。

[![img](https://user-images.githubusercontent.com/52620310/62405927-5e3a0400-b5d6-11e9-9b46-231b6b152909.jpg)](https://user-images.githubusercontent.com/52620310/62405927-5e3a0400-b5d6-11e9-9b46-231b6b152909.jpg)

完成以上步骤后就可以看到连接成功的界面，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405930-64c87b80-b5d6-11e9-9f01-3a5ab54e1dda.jpg)](https://user-images.githubusercontent.com/52620310/62405930-64c87b80-b5d6-11e9-9f01-3a5ab54e1dda.jpg)

**注意：**如果出现 Hostwinds 无法登录的情况，请参考以下解决办法：

#### 密码不对导致 Hostwinds VPS 连接不上

如果只是密码不对，显示 SSH 服务器拒绝了密码，如下图使用 Xshell 连接的显示示意图：

[![img](https://user-images.githubusercontent.com/52620310/62405932-698d2f80-b5d6-11e9-8c51-cd82d4997871.jpg)](https://user-images.githubusercontent.com/52620310/62405932-698d2f80-b5d6-11e9-8c51-cd82d4997871.jpg)

Hostwinds 采用 KVM，因此生成 Linux VPS 的密码的自动生成的，而 Hostwinds 发送的邮件中的密码可能不是VPS真实的密码，这时不知道密码是多少我们可以登录后台重新设置密码，步骤如下：

1、访问 <https://clients.hostwinds.com/clientarea.php>，点击你的 Service，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405941-86296780-b5d6-11e9-8a92-50bdf3d4091b.jpg)](https://user-images.githubusercontent.com/52620310/62405941-86296780-b5d6-11e9-8a92-50bdf3d4091b.jpg)

2、然后点击管理按钮，到管理界面，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405942-8aee1b80-b5d6-11e9-82ba-16510e9012a2.jpg)](https://user-images.githubusercontent.com/52620310/62405942-8aee1b80-b5d6-11e9-82ba-16510e9012a2.jpg)

3、然后点击修改密码按钮，在弹出框中重新输入密码，密码需要字母大小写、特殊符还有要一定长度：

[![img](https://user-images.githubusercontent.com/52620310/62405944-904b6600-b5d6-11e9-8d74-58896156e07b.jpg)](https://user-images.githubusercontent.com/52620310/62405944-904b6600-b5d6-11e9-8d74-58896156e07b.jpg)

4、修改后密码还没有生效，最关键的一步需要 重启服务器，才能生效，如下图所示点击重启：

[![img](https://user-images.githubusercontent.com/52620310/62405946-95a8b080-b5d6-11e9-80ea-e97308a31053.jpg)](https://user-images.githubusercontent.com/52620310/62405946-95a8b080-b5d6-11e9-80ea-e97308a31053.jpg)

这样就能够使用你就可以使用你设置的密码登录 Hostwinds VPS 了。

#### 如果是国内屏蔽导致 Hostwinds VPS 连接不上

我们都众所周知由于大陆的一些原因，国外 VPS 的 IP 是经常会被禁止的，如果被大陆屏蔽了，这种情况表现为可以 ping 通 IP，但是 SSH 连接不上。Hostwind VPS 是支持更换 IP。你可以通过 “Fix ISP Block” 功能来修复 IP，这个操作会自动修改 IP，具体操作我们具体看下。

打开 [Hostwinds 的官网](https://affiliates.hostwinds.com/hostwinds.php?id=7011&url=1224)，进入 Hostwinds 的后台控制面板：

[![img](https://user-images.githubusercontent.com/52620310/62405947-9b9e9180-b5d6-11e9-987e-a6a120eeacf2.jpg)](https://user-images.githubusercontent.com/52620310/62405947-9b9e9180-b5d6-11e9-987e-a6a120eeacf2.jpg)

然后输入用户名、密码登录

[![img](https://user-images.githubusercontent.com/52620310/62405949-a0634580-b5d6-11e9-96ea-4721c7d34d6c.jpg)](https://user-images.githubusercontent.com/52620310/62405949-a0634580-b5d6-11e9-96ea-4721c7d34d6c.jpg)

选择需要换 IP 的 VPS，点击绿色 “Manage” 按钮

[![img](https://user-images.githubusercontent.com/52620310/62405950-a6f1bd00-b5d6-11e9-93f5-05364f558811.jpg)](https://user-images.githubusercontent.com/52620310/62405950-a6f1bd00-b5d6-11e9-93f5-05364f558811.jpg)

然后点击 “Click Here to Manage This Server” 的按钮

[![img](https://user-images.githubusercontent.com/52620310/62405955-ac4f0780-b5d6-11e9-9fd7-7ba7fb1df86f.jpg)](https://user-images.githubusercontent.com/52620310/62405955-ac4f0780-b5d6-11e9-9fd7-7ba7fb1df86f.jpg)

点击 “Manage IPs” 按钮进行管理

[![img](https://user-images.githubusercontent.com/52620310/62405957-b113bb80-b5d6-11e9-9797-944039bc9af0.jpg)](https://user-images.githubusercontent.com/52620310/62405957-b113bb80-b5d6-11e9-9797-944039bc9af0.jpg)

然后点击 “Fix ISP Block” 按钮进行 IP 修复，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405960-b5d86f80-b5d6-11e9-98eb-3cc0ba9b076f.jpg)](https://user-images.githubusercontent.com/52620310/62405960-b5d86f80-b5d6-11e9-98eb-3cc0ba9b076f.jpg)

然后点击 “Confirm” 按钮确认

[![img](https://user-images.githubusercontent.com/52620310/62405961-bb35ba00-b5d6-11e9-9d6d-d9a91bc73f98.jpg)](https://user-images.githubusercontent.com/52620310/62405961-bb35ba00-b5d6-11e9-9d6d-d9a91bc73f98.jpg)

然后 Hostwinds VPS 的 IP 就会自动更换了，然后注意还需要**重装系统**才行，重装系统如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405969-c0930480-b5d6-11e9-9685-9e4eb8f21672.jpg)](https://user-images.githubusercontent.com/52620310/62405969-c0930480-b5d6-11e9-9685-9e4eb8f21672.jpg)

通过上面的方法就可以解决IP被屏蔽不能访问的问题了。

## 3、Hostwinds 安装 SSR 开始

在上图的待输入内容处，粘贴下面的命令（复制下面的命令，然后在 Xshell 待输入内容处“鼠标右键”/“粘贴”即可）：

```
yum -y install wget
wget -N –no-check-certificate https://raw.githubusercontent.com/ToyoDAdoubi/doubi/master/ssr.sh && chmod +x ssr.sh && bash ssr.sh
```

粘贴后会下载相关安装包，等待屏幕不动的时候按“回车键”，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405971-c5f04f00-b5d6-11e9-8347-343e29e69a29.jpg)](https://user-images.githubusercontent.com/52620310/62405971-c5f04f00-b5d6-11e9-8347-343e29e69a29.jpg)

然后等待一会儿，出现 SSR 安装的引导界面，输入数字1，按回车键进行 SSR 安装，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405974-cab50300-b5d6-11e9-92ef-28ba7701a5c1.jpg)](https://user-images.githubusercontent.com/52620310/62405974-cab50300-b5d6-11e9-92ef-28ba7701a5c1.jpg)

然后输入端口，尽量选择一个比较大的数字，避免端口冲突，建议选择 8099，经验证 8080、8090 端口是被封了的，千万不要用这个（如果后面遇到可以登录 VPS，但是 ssr 上不了网，可能就是端口封了，修改一下 ssr 端口就可以了）， 然后回车，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405976-d0124d80-b5d6-11e9-91dc-dba0511bea55.jpg)](https://user-images.githubusercontent.com/52620310/62405976-d0124d80-b5d6-11e9-91dc-dba0511bea55.jpg)

然后输入 SSR 账号的密码，随便输入一个密码，这里输入123qweasd，然后回车，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405978-d6082e80-b5d6-11e9-8ab2-c987c2a60129.jpg)](https://user-images.githubusercontent.com/52620310/62405978-d6082e80-b5d6-11e9-8ab2-c987c2a60129.jpg)

然后输入 SSR 账号的加密方式，随便输入 10，选择 aes-256-cfb 的加密方式，然后回车，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405979-dbfe0f80-b5d6-11e9-8238-bc7b391a1191.jpg)](https://user-images.githubusercontent.com/52620310/62405979-dbfe0f80-b5d6-11e9-8238-bc7b391a1191.jpg)

然后输入 SSR 账号的协议插件，随便输入 2，选择 auth_sha1_v4 的协议插件，然后回车，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405981-e0c2c380-b5d6-11e9-8b98-01d17b915e8f.jpg)](https://user-images.githubusercontent.com/52620310/62405981-e0c2c380-b5d6-11e9-8b98-01d17b915e8f.jpg)

然后选择是否设置协议插件兼容原版，随便输入 y，表示要设置，然后回车，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405984-e7513b00-b5d6-11e9-8580-e0dfeef1fdd5.jpg)](https://user-images.githubusercontent.com/52620310/62405984-e7513b00-b5d6-11e9-8580-e0dfeef1fdd5.jpg)

然后选择混淆插件，这里选择 1，然后回车，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405985-ec15ef00-b5d6-11e9-92a7-4756e17a332b.jpg)](https://user-images.githubusercontent.com/52620310/62405985-ec15ef00-b5d6-11e9-92a7-4756e17a332b.jpg)

然后设置限制的设备数，如果要限制就输入对于的数字，如果不限制就直接回车，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405989-f1733980-b5d6-11e9-8ce5-763ece4d8dee.jpg)](https://user-images.githubusercontent.com/52620310/62405989-f1733980-b5d6-11e9-8ce5-763ece4d8dee.jpg)

然后设置每个端口的速度，如果要限制就输入对于的数字，单位是 KB/S，如果不限制就直接回车，建议不限制速度，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405996-fb953800-b5d6-11e9-92dd-2908259317e5.jpg)](https://user-images.githubusercontent.com/52620310/62405996-fb953800-b5d6-11e9-92dd-2908259317e5.jpg)

然后设置总的速度，如果要限制就输入对于的数字，单位是 KB/S，如果不限制就直接回车，建议不限制速度，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62405997-0059ec00-b5d7-11e9-8e3e-af05163717a0.jpg)](https://user-images.githubusercontent.com/52620310/62405997-0059ec00-b5d7-11e9-8e3e-af05163717a0.jpg)

然后会开始部署，到下图所示的位置，提示你下载文件，输入：y

[![img](https://user-images.githubusercontent.com/52620310/62405999-05b73680-b5d7-11e9-82ad-04028d5af096.jpg)](https://user-images.githubusercontent.com/52620310/62405999-05b73680-b5d7-11e9-82ad-04028d5af096.jpg)

然后就耐心等待一会儿安装，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62406003-0c45ae00-b5d7-11e9-9ccf-6d949a2e177e.jpg)](https://user-images.githubusercontent.com/52620310/62406003-0c45ae00-b5d7-11e9-9ccf-6d949a2e177e.jpg)

等安装完成之后就可以看到 SSR 账号 配置信息，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62406005-110a6200-b5d7-11e9-8d87-bbf262b22218.jpg)](https://user-images.githubusercontent.com/52620310/62406005-110a6200-b5d7-11e9-8d87-bbf262b22218.jpg)

按照上面的图片就可以看到设置的 SSR 账号信息，包括 IP、端口、密码、加密方式、协议插件、混淆插件，这些信息都需要填入对应的 SSR 客户端。

## 4、Hostwinds 搭建 BBR 加速

虽然 SSR 搭建好了，但是速度还不是很快，要搭建 BBR 才快，下面我们就说说怎么搭建 BBR。

BBR 是 Google 的一款 SSR 加速产品，使用下面的命令就可以实现 BBR 加速，只有 [Hostwinds](https://affiliates.hostwinds.com/hostwinds.php?id=7011&url=1216) 等少数 KVM VPS 才支持 BBR 加速，这也是我们推荐选择 Hostwinds 的原因。

在 xShell 连接端输入，如下命令，然后回车：

```
yum -y install wget
wget –no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh
chmod +x bbr.sh
./bbr.sh
```

[![img](https://user-images.githubusercontent.com/52620310/62406006-18317000-b5d7-11e9-8146-b9b05d4240d7.jpg)](https://user-images.githubusercontent.com/52620310/62406006-18317000-b5d7-11e9-8146-b9b05d4240d7.jpg)

然后按任意键进行部署

[![img](https://user-images.githubusercontent.com/52620310/62406007-1c5d8d80-b5d7-11e9-822f-fd9ed195a88b.jpg)](https://user-images.githubusercontent.com/52620310/62406007-1c5d8d80-b5d7-11e9-822f-fd9ed195a88b.jpg)

然后需要等待命令执行，大约5分钟，如下图所示：

[![img](https://user-images.githubusercontent.com/52620310/62406009-22536e80-b5d7-11e9-826b-e1f1b0774db9.jpg)](https://user-images.githubusercontent.com/52620310/62406009-22536e80-b5d7-11e9-826b-e1f1b0774db9.jpg)

会在下面的图片过程中等待一会儿

[![img](https://user-images.githubusercontent.com/52620310/62406011-267f8c00-b5d7-11e9-8ac1-67599ff1facb.jpg)](https://user-images.githubusercontent.com/52620310/62406011-267f8c00-b5d7-11e9-8ac1-67599ff1facb.jpg)

最后完成后需要重启，根据提示输入：y，重启服务器即可生效

[![img](https://user-images.githubusercontent.com/52620310/62406015-2bdcd680-b5d7-11e9-9aec-fdf762a5f191.jpg)](https://user-images.githubusercontent.com/52620310/62406015-2bdcd680-b5d7-11e9-9aec-fdf762a5f191.jpg)

如果错过了重启步骤，直接输入重启命令命令：

```
reboot
```

[![img](https://user-images.githubusercontent.com/52620310/62406018-31d2b780-b5d7-11e9-819b-baa65e585c47.jpg)](https://user-images.githubusercontent.com/52620310/62406018-31d2b780-b5d7-11e9-819b-baa65e585c47.jpg)

然后耐心等待，待服务器重启后即可自动开启 SSR 加速。(这里注意如果是 centos 7 系统重启后可能防火墙阻止了 SSR，需要关闭防火墙，如果是 centos 6 就不会有这个问题，所以我们建议使用的是 Hostwinds 的 centos 6 操作系统。)

## 5、Hostwinds 搭建 SSR 总结

怎样使用 SSR 各种平台客户端这里就不详细介绍了。

以上就是美国 VPS Hostwinds 搭建 SSR 的教程，通过教可以轻松实现 Hostwinds 搭建 SSR，希望可以帮助需要使用 Hostwinds 搭建 SSR 的朋友。

[Hostwinds 最好美国VPS低至4.49美元/月](https://affiliates.hostwinds.com/hostwinds.php?id=7011&url=1216)，支持支付宝付款，欢迎购买注册。
