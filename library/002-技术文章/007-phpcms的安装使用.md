## PHPCMS的安装流程

1. 本地服务器www目录下新建文件phpcms

2. 在网站www.phpcms.cn下载安装包。
有GBK 和 UTF8两个版本，推荐使用UTF8版本。下载文件解压，删除readme文件夹，将install_package文件夹下的文件拷贝到www目录下的phpcms文件夹内

3. 访问localhost/phpcms/install/install.php按照指导进行安装

![phpcms安装](assets/002/007-9d5257eb.png)

不懂本教程，没关系，查看 [详细教程](http://www.jianshu.com/p/b1a42f63965a)

注：后台管理系统中的设置可修改默认站点域名

![](assets/002/007-646f87bd.png)

#### 三个重要的地址

localhost/phpcms/admin.php(后台管理系统 账号：phpcms 密码：phpcms)

localhost/phpcms/index.php(前台首页文件)

localhost/phpcms/myadmin(数据库)

#### 两个重要的目录
1. www/phpcms/phpcms/tmplates/default/content/

2. www/phpcms/statics/ -css/ -images/ -js/
