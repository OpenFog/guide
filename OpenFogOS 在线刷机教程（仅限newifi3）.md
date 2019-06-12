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



4. 进行解锁。 
（1）输入 cd /tmp 
（2）输入 wget https://download.openfogos.com/newifi3/newifi_jail_break.ko
等待下载完成，如图。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190103182924455.png)



(3) 输入 insmod newifi_jail_break.ko 进行解锁。
（4) 解锁完成后会进行重启。
5. 刷机 
（1）输入 cd /tmp 
（2）输入 wget https://download.openfogos.com/newifi3/firmware.bin
等待下载完成，如图。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190103182943159.png)

（3）输入mtd -r write firmware.bin firmware 
（4）显示如图则表示刷机成功，刷机完成重启需要等待较长时间（大约1-2分钟）
![在这里插入图片描述](https://img-blog.csdnimg.cn/2019010318301743.png)



6. 在浏览器中输入192.168.99.1 若显示页面如图则表示刷机成功（默认密码admin)。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190103183024149.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)