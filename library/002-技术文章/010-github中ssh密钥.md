## github中ssh密钥的生成（如何不用输密码同github交互）

### 1. 查看SSH keys是否存在

打开git Brash界面--》输入 ssh

如果出现如下界面，代表SSH keys存在

![](assets/002/010-e55e0343.png)

### 2. 生成新的ssh key

在命令行中输入`ssh-keygen -t rsa -C "3396543978@qq.com"`

输入passphrase（本步骤可以跳过）不输入则表示没有密码

将新生成的key添加到ssh-agent中:

![](assets/002/010-b7565b9a.png)

如果出现如下界面，则创建成功

![](assets/002/010-81e4590a.png)

### 3. 将ssh key添加到Github中

用自己喜欢的文本编辑器打开id_rsa.pub文件，里面的信息即为SSH key，将这些信息复制到GitHub的Add SSH key页面即可
