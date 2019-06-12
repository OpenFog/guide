
1. ssh登录进入路由器中。（以在Windows中XShell为例，路由器的地址为192.168.1.1）
   （1）输入 ssh root@192.168.1.1
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190130173357274.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)
 （2）点击接受并保存，会弹出输入密码窗口，在窗口中输入密码。（默认密码为：admin）
 ![在这里插入图片描述](https://img-blog.csdnimg.cn/20190130173523965.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)
 （3）如图所示即登录成功。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190130174303287.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)
2. 依赖安装。
（1）输入opkg update    回车，出现如图所示类似效果表示成功。
  ![在这里插入图片描述](https://img-blog.csdnimg.cn/20190130174558410.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)
（2）输入 opkg install libcurl  wget 回车，出现类似如图所示表示成功。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190130184023349.png)
3. 安装ipk。
（1）输入 cd /tmp
（2）输入 wget --no-check-certificate https://download.openfogos.com/pandorabox/openfogos.ipk
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190130184420362.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)
（3）输入 opkg install openfogos.ipk
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190130181539260.png)
 （4) 输入 /etc/init.d/xc_cdn enable
 ![在这里插入图片描述](https://img-blog.csdnimg.cn/20190215102047882.png)
如图所示即安装成功。
4. 拔电重启路由器，完成ipk安装。
  https://i.openfogos.com  注册账户绑定设备领取收益。