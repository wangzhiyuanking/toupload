1、新建仓库

<img src="README.assets/image-20201203200521356.png" alt="image-20201203200521356" style="zoom: 67%;" />

尽量不要自动添加README.md



所使用的电脑与github进行SSH连接

<img src="README.assets/image-20201203200743770.png" alt="image-20201203200743770" style="zoom:67%;" />

生成密钥

命令：ssh-keygen -t rsa -C "2656489919@qq.com"，连续按enter键

<img src="README.assets/image-20201203201108377.png" alt="image-20201203201108377" style="zoom:67%;" />![image-20201203201244554](README.assets/image-20201203201244554.png)

![image-20201203201244554](README.assets/image-20201203201244554.png)

<img src="README.assets/image-20201203201358418.png" alt="image-20201203201358418" style="zoom:67%;" />

<img src="README.assets/image-20201203201507314.png" alt="image-20201203201507314" style="zoom:67%;" />

电脑已经和github进行了连接，可以相互通信了，测试是否连接成功代码 ssh -T git@github.com

![image-20201203202422277](README.assets/image-20201203202422277.png)

![image-20201203202523246](README.assets/image-20201203202523246.png)

电脑端配置，确定是谁上传的

```
git config --global user.name wangzhiyuan
git config --global user.email 2656489919
```





2、初始化仓库

```
git init
```

3、让git管理文件（使用.管理目录下的所有文件）

```
git add .
```

4、将文件提交到本地仓库中

```
git commit -m "对本次提交进行文字说明"
```

5、对已经存在的分支重命名

```
git branch -M main
```

6、关联远程github上的仓库

```
git remote add origin git@github.com:wangzhiyuanking/toupload.git
```

7、将本地仓库内容推到远程github仓库

```
git push -u origin main
```

更新代码到github上(一定要切换到项目目录上)

![image-20201203203901402](README.assets/image-20201203203901402.png)

![image-20201203203929589](README.assets/image-20201203203929589.png)