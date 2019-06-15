1. 确保电脑连在路由器下，路由器和电脑可以正常联网。


2. 开启SSH后门。
（1）打开电脑浏览器，在地址栏输入192.168.99.1，界面如图。

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190103182405363.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)
（2) 在浏览器中输入 http://192.168.99.1/newifi/ifiwen_hss.html
若返回success则表示开启SSH成功。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190103182418834.png)

3. 进入路由器SSH环境，以Windows下使用Xshell为例。
（1）安装Xshell，打开。
（2）输入 ssh root@192.168.99.1，回车（enter)，会出现如图所示界面。

![在这里插入图片描述](https://img-blog.csdnimg.cn/2019010318251717.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)
（3) 点击接受并保存，出现如图所示页面。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190103182535231.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)

（4) 输入你的路由器后台管理密码（一般与路由器WiFi密码相同），点击确定，出现如图所示页面，表示ssh登录成功。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190103182904271.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)

4. 安装ipk。
（1）输入 cd /tmp 回车。
（2）输入 wget https://download.openfogos.com/newifi3/openfogos.ipk
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190122171639830.png)
（3）输入 opkg --force-overwrite install openfogos.ipk
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190122171755173.png)
即安装成功，重启路由器后即可在  https://i.openfogos.com 中绑定。

