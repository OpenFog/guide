0. 安装前确认设备已经连接至互联网，并在安装过程中一直保持联网。
确认设备为[已支持设备列表](https://blog.csdn.net/weixin_44388511/article/details/87881369)中的设备(MTK7620系列)，PandoraBox版本为18.07及以上。（在 状态>系统中可以看到）

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190225143232360.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)
1. ssh登录进入路由器中。（以在Windows中XShell为例，路由器的地址为192.168.1.1）
   （1）输入 ssh root@192.168.1.1
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190130173357274.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)
 （2）点击接受并保存，会弹出输入密码窗口，在窗口中输入密码。（默认密码为：admin）
 ![在这里插入图片描述](https://img-blog.csdnimg.cn/20190130173523965.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)
 （3）如图所示即登录成功。
![在这里插入图片描述](https://img-blog.csdnimg.cn/2019022514334132.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)
2. 依赖安装。
（1）输入opkg update    回车，出现如图所示类似效果表示成功。
  ![在这里插入图片描述](https://img-blog.csdnimg.cn/20190225143427489.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)
（2）输入 opkg install  curl  libcurl  回车，出现类似如图所示表示成功。
![在这里插入图片描述](https://img-blog.csdnimg.cn/2019022514422235.png)
3. 安装ipk。
（1）输入 cd /tmp
（2）输入 curl -k https://download.openfogos.com/youku/openfogos.ipk -o openfogos.ipk
![在这里插入图片描述](https://img-blog.csdnimg.cn/2019022514445782.png)
（3）输入 opkg install openfogos.ipk
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190225144606110.png)
 （4) 输入 /etc/init.d/xc_cdn enable
 ![在这里插入图片描述](https://img-blog.csdnimg.cn/20190215102047882.png)
如图所示即安装成功。
4. 拔电重启路由器，完成ipk安装。
  https://i.openfogos.com  注册账户绑定设备领取收益。