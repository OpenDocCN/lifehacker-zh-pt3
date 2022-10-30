# 用 OS X Server 将旧 Mac 变成廉价的 VPN

> 原文:[https://life hacker . com/turn-an-old-MAC-into-a-cheap-VPN-with-OS-x-server-1743411938](https://lifehacker.com/turn-an-old-mac-into-a-cheap-vpn-with-os-x-server-1743411938)

虚拟专用网订阅是要花钱的，而且他们通常需要一点研究来确定他们是否合法 。如果你有一台旧的 Mac，你可以把它变成最简单的 DIY VPN，非常适合在公共 Wi-Fi 上安全浏览或在旅途中从家里的电脑上抓取文件。

Watch

### 你会得到什么

对于那些不知道的人来说，VPN 代表虚拟专用网络。VPN 是一组通过公共网络(通常是互联网)联网在一起的计算机。你的办公室可能会使用 VPN，这样你就可以从家里访问你的工作电脑，但它们也有助于在咖啡店或酒店的 [公共 Wi-Fi 上保持安全。](https://lifehacker.com/how-to-stay-safe-on-public-wi-fi-networks-5576927)T3】

当你完成这个项目时，你将拥有自己的个人 VPN，可以从任何计算机访问，无论是在家庭网络上还是在家庭网络外。你的虚拟专用网将能够作为一种安全的手段来浏览网页 并从任何地方连接到你的家庭网络，因此无论你在世界的任何地方，你都可以访问你的文件。你可以用一个 20 美元的软件来完成所有这些工作，这个软件可以在任何 T4 的 Mac 电脑上运行。

另外，这非常简单。运行自己的 VPN 通常意味着经历令人挠头的 OpenVPN 设置，但是 OS X Server 极大地简化了这个过程——你甚至不必进入命令行。如果你有一台旧的苹果电脑，坐在那里收集灰尘，花 20 美元在软件上，你可以让这个虚拟专用网立刻运行起来。

<aside class="sc-1rh3ayr-6 eaNzNC inset--story branded-item branded-item--lifehacker" data-commerce-source="inset">[![Image for article titled Turn an Old Mac Into a Cheap VPN with OS X Server](../Images/aef335eb562a1da6957ce25a574b4aa1.png)](https://lifehacker.com/how-to-stay-safe-on-public-wi-fi-networks-5576927) [###### 如何在公共 Wi-Fi 网络上保持安全](https://lifehacker.com/how-to-stay-safe-on-public-wi-fi-networks-5576927) 

公共 Wi-Fi 网络——如咖啡店或酒店中的网络——远没有你想象的那么安全。…

[Read more](https://lifehacker.com/how-to-stay-safe-on-public-wi-fi-networks-5576927)</aside>

### 你需要什么

*   [OS X 服务器](https://itunes.apple.com/us/app/os-x-server/id883878097?mt=12)(19.99 美元)
*   一台备用的 Mac(任何 Mac 都可以，但如果你没有的话，通常可以在易贝找到一台价格约为 100 美元 的旧的、便宜的 Mac Mini。只要确保它满足 OS X El Capitan 的 [最低要求即可)](https://support.apple.com/kb/SP728?locale=en_US)
*   以太网电缆、路由器(我们推荐普通路由器 ，而不是路由器/调制解调器组合)和互联网连接

### 第一步:插入所有东西并下载 OS X Server

您需要在 Mac 和路由器之间建立硬连线连接，以获得最快、最可靠的连接，因此在您做任何其他事情之前，请使用以太网电缆将 Mac 插入路由器。

之后，如果你还没有升级到 OS X El Capitan 的话，去你的旧 Mac 上的苹果应用商店升级到 [。然后，从 App Store 中抓取一份](https://itunes.apple.com/WebObjects/MZStore.woa/wa/viewSoftware?id=1018109117&mt=12&ls=1) [OS X Server](https://itunes.apple.com/us/app/os-x-server/id883878097?mt=12) 。OS X Server 只是一个应用程序，而不是一个成熟的操作系统，所以安装应该是一键操作。

如果你的 Mac 不支持 El Capitan，你可能仍然可以 [在这里](https://support.apple.com/en-us/HT203137) 下载 OS X Server，但我们没有用 OS X 的每个版本测试这些指令，所以它们可能会略有不同。基本上，你的里程可能会有所不同。

### 第二步:注册一个动态 DNS 地址

接下来，您需要为您的旧 Mac 获取一个公共 DNS 地址，以便远程访问您的服务器。您可以使用您家的 IP 地址(例如 12.345.678.9)，但是您的 ISP 可能会定期更改该 IP 地址，这使得域名(jimsVPN.crabdance.com)成为一个更好的选择——它容易记忆，并且总是相同的。

如果你有自己的网站，很有可能你的域名提供商免费提供动态域名服务；否则，你需要注册一项服务。我们推荐 [FreeDNS](http://freedns.afraid.org/menu/) 因为它是免费的， [但是你有其他选择](https://lifehacker.com/the-best-free-alternatives-to-dyndns-1561556205) 。

1.  在免费域名系统 上注册 [账户，并验证你的电子邮件地址。](http://freedns.afraid.org/signup/)
2.  点击 [动态 DNS](http://freedns.afraid.org/dynamic/) 。
3.  单击添加。
4.  键入一个子域名(这可以是您想要的任何名称，但为了简单起见，您可能希望使用类似于 jimssecretVPN 的名称)，然后单击您想要的域名(同样，这可以是任何名称)。
5.  单击保存。
6.  记下您的域名(类似于 jimssecretvpn . crabtance . com)。

您现在有了一个永久的 VPN 地址，因此您可以从世界上任何网络上的任何计算机拨号进入。

### 第三步:在路由器上设置端口转发

在 OS X Server 上设置 VPN 之前，您需要将路由器设定为允许正确端口上的传入连接。为此，您将启用*端口转发*。这是最复杂的部分，因为每个路由器的流程都不一样。我们已经在 [中深入介绍了如何设置端口转发，在这里](http://lifehacker.com/know-your-network-lesson-4-access-your-home-computers-5831841#portforwarding&_ga=1.261117837.1055861349.1441835238) 中，我们先来大致了解一下这个过程:

1.  从网络浏览器进入路由器的管理页面。这通常是类似于`192.168.1.1`的东西。如果你不确定你的是什么，你通常可以在你的路由器上的标签上找到信息(如果没有，请参考你的路由器手册或在谷歌上搜索)。
2.  找到 DHCP 或静态租用部分。在我们做任何事情之前，你需要给你的 Mac 一个 DHCP 预留(有时称为静态租用)，这样它的本地 IP 地址就不会改变。这个过程因路由器而异，但是 [我们在这里](http://lifehacker.com/how-to-set-up-dhcp-reservations-and-never-check-an-ip-5822605) 概述了如何做。如果你的路由器没有这个选项，你可以 [给你的 Mac 一个静态 IP 地址来代替](http://www.howtogeek.com/howto/22161/how-to-set-up-a-static-ip-in-mac-os-x/) 。记下 Mac 的新 IP 地址，因为下面会用到它。
3.  现在，找到端口转发部分。根据您的路由器和固件，它通常位于自己的标签、防火墙、NAT 或虚拟服务器下。
4.  这是您将启用端口转发的地方。在端口转发页面上，您通常会找到一个地方来输入信息，如端口 From、协议、IP 地址和端口 to。OS X Server 的 VPN 需要打开四个端口才能工作:UDP 500、UDP 1701、TCP 1723 和 UDP 4500。添加这四个端口，如上面的示例截图所示。完成后保存您的设置。

这样，您的家庭 VPN 服务器现在对互联网开放，因此您可以从任何地方访问它。让我们让其余的工作。

### 第四步:设置你的服务器

还记得我们之前设置的动态 DNS 帐户吗？现在，您需要在 Mac 上启用它，以便出门在外时可以连接到它:

1.  在旧 Mac 上启动 OS X Server。
2.  从左侧菜单中单击您的计算机名称。
3.  单击“编辑主机名...”并在出现提示时单击下一步。
4.  单击 Internet，然后单击下一步。
5.  在主机名下，键入您在第二步中注册的域名，然后单击完成。
6.  出现提示时，点按“设置 DNS”并让它自动启动和配置 DNS。您不需要更改这些设置。

这就是服务器部分。OS X Server 的自动配置应该适用于大多数人。

### 第五步:启动你的 VPN

现在是时候最终启动并运行 VPN 了。这部分很简单:

1.  在 OS X Server 的边栏中点按“VPN”部分。
2.  默认设置应该已经填充了您需要的大部分内容，但是如果没有，请确保您的 VPN 主机名与您在第四步中输入的主机名相同。
3.  创建一个“共享秘密”密码。在此处设置一个便于记忆的密码，您需要在尝试连接的任何设备上输入该密码。
4.  找到“客户端地址”部分，然后单击“编辑地址”这些是您的服务器将分配给连接到 VPN 的计算机的 IP 地址。默认情况下，它应该已经输入了您的网络的 IP 地址(类似于`192.168.1.xx`)。将最后三个数字设置得高一些，比如 100，这样它就显示为`192.168.1.100`(或者你的网络)。这将防止 VPN 连接的任何问题干扰网络上的其他连接。
5.  将 VPN 切换到“开”

大约 10-20 秒后，状态应该切换到[您的主机名]上的“可用”。这意味着你已经准备好了。

### 如何从其他设备访问您的 VPN

现在，您的 VPN 已经启动并运行，您需要设置其他计算机和移动设备来通过它路由流量。请记住，VPN 会降低您的互联网连接速度，因此只在需要时使用它，例如当您在不安全的公共网络上时，或者当您需要从家庭网络访问文件时。

您需要分别设置每台设备。无论您从哪里连接，您的帐户信息总是相同的。您的用户名是您用来登录 Mac 的用户名，密码是您 Mac 的登录密码。您还有“共享密码”，这是您在第五步中设置的第二个密码。这一过程因设备而异，但基本情况如下:

**Windows 10**

1.  单击开始>设置。
2.  开放网络和互联网。
3.  点击 VPN。
4.  单击添加 VPN 连接。
5.  用您的 VPN 信息填写表单，包括您在第一步中设置的公共 IP 地址、您的密码、帐户和共享密钥。完成后，单击保存。
6.  选择您创建的 VPN，然后单击连接。

**Mac**

1.  打开“系统偏好设置”>“网络”。
2.  单击+号。
3.  选择 VPN，然后选择 L2TP。
4.  输入您的服务器地址和帐户名称，然后点按“鉴定设置”。
5.  输入您的密码和共享密码，然后单击确定。
6.  单击连接。

**iOS**

1.  轻按“设置”>“通用”>“VPN”。
2.  点击添加 VPN 配置。
3.  输入您的所有帐户信息，包括类型(L2TP)、服务器、帐户、共享密钥和密码。
4.  点击保存。
5.  将状态设置为开。

**安卓**

1.  点击设置>无线和网络设置> VPN 设置。
2.  选择基本 VPN，然后添加 VPN。
3.  选择添加 L2TP/IPSec PSK VPN。
4.  输入您的服务器地址、帐户信息、共享密钥和密码。

恭喜你！您的 VPN 已启动并运行，并且您的所有设备都通过它安全地路由流量。您可以随时在 OS X Server 中的“VPN”标签下或电脑名称下的“概述”标签上检查 VPN 的状态。

尼克·克里斯库洛的动画。T3】