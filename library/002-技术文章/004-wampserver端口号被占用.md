## 解决WampServer 80端口号被占用的问题

- #### 沿着C:\wamp\bin\apache\apache2.4.9\conf目录，找到文件httpd.conf文件

  将80端口号改为任意值，诸如8080端口：

![](assets/002/004-c607ac52.png)

![](assets/002/004-934c4be8.png)

  改完之后重启WampServer就会发现软件图标变为了绿色

  但是“Localhost”、“phpMyAdmin”、“SQLiteManager”，你可以点击打开看到依旧是默认的80端口。

- #### 找到wamp安装目录下的wampmanager.tpl文件，记事本打开：

![](assets/002/004-4af22449.png)

![](assets/002/004-2df03c4e.png)

- #### 找到wamp安装目录下的wampmanager.ini文件

`将本文件中的http://localhost 替换为 http://localhost:8080`

![](assets/002/004-a8469be9.png)

![](assets/002/004-3e357bd6.png)

![](assets/002/004-b27f7da2.png)
