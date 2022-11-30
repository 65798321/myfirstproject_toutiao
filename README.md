# 我的第一个项目

#### 项目准备：

##### 1.安装脚手架环境 --

​	vue create myproject

​	cd /myproject

​	npm run serve

​				

##### 2.安装git 使用git 进行版本控制

​	git init 初始化项目，在项目第一层文件夹控制台执行该命令会创建一个.git文件夹，里面有相应配置[](D:\qianduan\bij\00-笔记课件资料\04-第四阶段\04-阶段四：前后端交互阶段资料新\第四阶段：前后端交互阶段资料新\Git+github\day02（5-7小节）\讲义（pdf）\00_Git.pdf)



​	![image-20221130112420438](C:\Users\asd\AppData\Roaming\Typora\typora-user-images\image-20221130112420438.png)

​	git 工作区（init之后的文件夹都为工作区）文件的四种状态：

​		1.未跟踪 此时的文件是不被git管理，就是git不会监控这些文件，此时运行git status -s 是无法发现未跟踪文件 显示的文件前面有红色的问号

​		2.未修改 此时工作区中文件的内容和git仓库中保持一致，执行git status -s  显示的文件前面有绿色的A标记

​		3.已修改 工作区中中文件和git仓库中文件的内容不一致，执行git status -s 显示的文件前面有红色的M

​		4.已暂存工作区中被修改的文件已被放到暂存区，准备将修改后的文件保存到git仓库中,显示的文件夹前面有绿色的M



​	git的基本操作：

​		1.检查文件的状态:git status 检查状态，git status -s快捷检查，文件前面会有对应的字母符号显示文件状态

​		2.跟踪新文件 git add 文件名，跟踪所有文件git add -A或者git add .

​		3.提交更新 git commit -m "提交消息"

​		4.暂存已修改的文件 git add 文件名 暂存所有文件 git add -A 该命令是个多功能命令 ，根据目标文件的状态不同，此命令的效果也不同，可以用来：开始跟踪新文件、把已跟踪的文件放到暂存区还能用于合并时把有冲突的文件标记为已解决状态

​		5.提交已暂存的文件 git commit -m "提交消息" ，此时是提交到git仓库中保存

​		6.跳过使用暂存区  	Git 标准的工作流程是工作区 → 暂存区 → Git 仓库，但有时候这么做略显繁琐，此时可以跳过暂存区，直接将工作区中的修改提交到 Git 仓库，这时候 Git 工作的流程简化为了工作区 → Git 仓库   使用方法：git commit -a 就可以跳过git add



​	github远程仓库管理

​		进入github新建空白远程仓库

​		![image-20221130150017354](C:\Users\asd\AppData\Roaming\Typora\typora-user-images\image-20221130150017354.png)



​	通过ssh key使用远程仓库

![image-20221130150129449](C:\Users\asd\AppData\Roaming\Typora\typora-user-images\image-20221130150129449.png)

​	生成ssh key

![image-20221130150212872](C:\Users\asd\AppData\Roaming\Typora\typora-user-images\image-20221130150212872.png)

​	配置ssh key

![image-20221130150237094](C:\Users\asd\AppData\Roaming\Typora\typora-user-images\image-20221130150237094.png)

​	检测github的ssh key是否配置成功

​	![image-20221130150307511](C:\Users\asd\AppData\Roaming\Typora\typora-user-images\image-20221130150307511.png)

​	基于ssh将本地仓库上传到github

​	![image-20221130150332950](C:\Users\asd\AppData\Roaming\Typora\typora-user-images\image-20221130150332950.png)
