# 同时push到多个远程仓库

### 以同时push到码云和github为例

1. 码云建立一个空仓库

   `如git地址为 https://gitee.com/qiangxuelixing/gitbook.git`

2. github建立一个空仓库

   `如git地址为 https://github.com/qiangxuelixing/gitbook.git`

3. 在本地创建一个项目

4. 把本地项目初始化git

   `git init`

   <font color=red>第3步也可以从码云或者github克隆下来，这样就不需要第4步的处理了</font>

5. 随便修改点什么，以便稍后push

   ```
   git add README.md # 以修改并提及README.md文件为例
   git commit -m "first commit"
   git remote add origin 码云的仓库地址
   git remote set-url --add origin github的仓库地址
   ```

6. push

   ```
   git push -u origin master # 按提示依次输入码云和github的用户名密码即可
   ```

   