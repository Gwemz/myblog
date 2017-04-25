## wamp下apache2.4.9局域网ip访问时提示403错误

在自己的笔记本上搭建了一个apache服务器，想通过手机访问主机上的一个页面，但是在访问过程中总提示403错误。
经过在网上查找别人的解决方案，及不断尝试修改httpd.conf配置文件，最终测试出修改方案。

找到(目录C:\wamp\bin\apache\apache2.4.9\conf下的httpd.conf文件)
```
<Directory>
Require local
</Directory>
```
将

**Require local**

修改为

**Require all granted**

真心是尝试过很多修改方法，网友们也说去修改什么allow from all类似这种，都有尝试过。可能是版本不同吧，本方法经测试OK，希望对大家有帮助。
