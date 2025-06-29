# 					R+BlogDown问题解决

1、Git的下载

2、hugo的下载

[Releases · gohugoio/hugo](https://github.com/gohugoio/hugo/releases)![](C:\Users\c2027\AppData\Roaming\Typora\typora-user-images\image-20250627235934799.png)

3、RStudio的下载

4、R的下载



5、无穷循环的解决

```
# 查看是否有用户配置文件导致递归
file.exists("~/.Rprofile")  # 检查主目录是否有配置文件

# 临时重命名测试
file.rename("~/.Rprofile", "~/.Rprofile_backup")  # 重命名后重启R

# 如果是RStudio项目，检查项目目录的.Rprofile
file.exists(".Rprofile")  # 项目目录
```

![image-20250628001023044](C:\Users\c2027\AppData\Roaming\Typora\typora-user-images\image-20250628001023044.png)

6、克隆失败解决

##### 1. 设置 Git 全局代理（替换实际代理）
git config --global http.proxy http://127.0.0.1:7890
git config --global https.proxy https://127.0.0.1:7890

##### 2. 重试克隆

git clone https://github.com/Mc-Flighting/ckw.git



##### 1. 用管理员身份编辑 C:\Windows\System32\drivers\etc\hosts
##### 2. 添加行：
140.82.113.4 github.com

##### 3. 刷新 DNS
ipconfig /flushdns

![image-20250628000404842](C:\Users\c2027\AppData\Roaming\Typora\typora-user-images\image-20250628000404842.png)

![image-20250628000450189](C:\Users\c2027\AppData\Roaming\Typora\typora-user-images\image-20250628000450189.png)