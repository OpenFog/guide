以 Ubuntu 18.04 安装为例。

 1.  打开terminal。

 3. 开启root权限，输入
```
sudo  -i 
```
输入密码，如图
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190507162146505.png)
 
 3. 下载安装程序，输入
 

```
wget https://download.openfogos.com/linux/openfog
```
 ![在这里插入图片描述](https://img-blog.csdnimg.cn/20190507162612631.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NDM4ODUxMQ==,size_16,color_FFFFFF,t_70)
 
 4. 赋给文件运行的权限，输入

```
chmod 777 openfog
```
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190507162713152.png)

 5. 运行安装程序，输入  
 ```
 ./openfog
 ```
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190507163904232.png)

 6.   如图所示即为安装成功。
 ![在这里插入图片描述](https://img-blog.csdnimg.cn/20190507163936131.png)
7. 常见问题
有时运行第五步会遇到下载速度很慢或者下载失败，是因为同时下载安装的人太多或者国外下载源不稳定的原因，此时需要先运行以下命令：（切换下载地址为国内镜像源下载）

```
  sudo echo "DOCKER_OPTS=\"--registry-mirror=http://hub-mirror.c.163.com\"" >> /etc/default/docker && \
  sudo service docker restart
```
