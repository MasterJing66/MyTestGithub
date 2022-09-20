# Git

## 1.创建一个文件夹

![image-20220913204221951](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220913204221951.png)

## 2.打开Git终端：

Git Bash Here:

进入以后先对字体和编码进行设置：

![image-20220913203233480](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220913203233480.png)

![image-20220913203313329](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220913203313329.png)

在Git中命令跟Linux是一样的：

（1）查看git安装版本：

![image-20220913203520081](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220913203520081.png)

（2）清屏

![image-20220913203556906](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220913203556906.png)

（3）设置签名：

设置用户名和邮箱：

![image-20220913203800058](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220913203800058.png)

![image-20220913203914432](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220913203914432.png)

（4）本地仓库的初始化操作：

通过输入路径进入对应的GitResp文件夹，再进行初始化操作

![image-20220913215940288](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220913215940288.png)

.git目录是隐藏的：可以调出来查看：

查看目录下隐藏文件

![image-20220913220231948](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220913220231948.png)

![image-20220913220200524](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220913220200524.png)

![image-20220913220637702](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220913220637702.png)

## 3.add和commit命令

展示：

（1）先创建一个文件

![image-20220913220841956](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220913220841956.png)

（2）将文件提交到暂存区

![image-20220914103623264](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914103623264.png)

（3）将暂存区的内容提交到本地库

![image-20220914103713044](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914103713044.png)

注意事项 ![image-20220914103932477](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914103932477.png)

![image-20220914104007368](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914104007368.png)

报错：在d盘根目录下没有配置本地仓库，提交的文件必须到本地仓库所在路径下

（1）不放在本地仓库中的文件，git是不进行管理的

（2）即使放在本地仓库的文件，git也不管理，必须通过add，commit命令操作才可以将内容提交到本地库。

## 4.git status看的是工作区和暂存区的状态

在GitResp目录下新建一个Demo2.txt，然后查看状态

![image-20220914185525556](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914185525556.png)

然后将Demo2.txt通过git add命令提交至：暂存区

![image-20220914185744295](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914185744295.png)

查看状态：

![image-20220914185828040](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914185828040.png)

利用 git commit 命令将文件提交至：本地库

![image-20220914190059405](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914190059405.png)

现在修改Demo2.txt文件中内容

![image-20220914190253501](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914190253501.png)

然后再查看状态

![image-20220914190424849](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914190424849.png)

重新添加至暂存区：查看状态

![image-20220914190613543](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914190613543.png)

将暂存的文件提交至本地库：显示Demo2.txt增加了五行

![image-20220914190855041](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914190855041.png)

提交完再查看状态：

![image-20220914191016073](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914191016073.png)

## 5.git log 可以让我们查看提交的文件，显示从最近到最远的日志

![image-20220914193908234](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914193908234.png)

## 6.git log 相关命令

当历史记录过多的时候，查看日志的时候，有分页效果，一页展示不下：

![image-20220914195647383](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914195647383.png)

有：说明可以往下走 （下一页：空格 ，上一页：b）,到尾页显示END![image-20220914200009736](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914200009736.png)，

退出END状态（按q),回到命令行

日志展示方式：

### 【1】方式1：git log -->分页

### 【2】方式2：git log --pretty=oneline

![image-20220914200313144](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914200313144.png)

### 【3】方式3：git log --oneline

![image-20220914200410864](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914200410864.png)

### 【4】方式4：git reflog

多了信息：HEAD@{数字}，这个数字的含义：指针回到当前这个历史版本需要多少步

![image-20220914200735252](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914200735252.png)

## 7.reset命令：前进或者后退历史版本

复制key：直接选中索引即可复制  <img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914202635745.png" alt="image-20220914202635745" style="zoom: 67%;" />

然后通过右键<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914202824459.png" alt="image-20220914202824459" style="zoom: 50%;" />

通过 git reset --hard [索引]值即可到达指定版本

![image-20220914203053733](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914203053733.png)

回退到版本HEAD@{5} ,即此时的Test.txt文件中只有aaaaaa

![image-20220914203318163](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914203318163.png)

查看Test.txt:

![image-20220914203233669](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914203233669.png)

### 【1】hard参数

git reset --hard[索引]

本地库的指针移动的同时，重置暂存区，重置工作区

### 【2】mix参数

本地库移动的同时，重置暂存区，但是工作区不重置

### 【3】soft参数

本地库的指针移动的同时，暂存区和工作区不动

总结：一般使用第一种hard参数

## 8.删除命令

### 【1】新建一个Test1.txt文件

### 【2】将它add到暂存区

### 【3】在通过commit提交到本地库



![image-20220914205142763](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914205142763.png)

![image-20220914205424500](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914205424500.png)

### 【4】删除工作区中的Test1.txt

![image-20220914205157627](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914205157627.png)

![image-20220914205204311](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914205204311.png)

### 【5】将删除操作同步到暂存区：

![image-20220914205735260](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914205735260.png)

### 【6】将删除操作同步到本地库：

![image-20220914205841966](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914205841966.png)

### 【7】查看日志

![image-20220914210318674](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914210318674.png)

### 【8】找回本地库删除的文件，实际上就是将历史版本切换到刚才添加文件的哪个版本即可

![image-20220914210348758](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914210348758.png)

![image-20220914210444574](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220914210444574.png)

## 9.diff命令

### git diff [文件名]

【1】先创建一个文件test2.txt，添加到缓存区，再提交到本地库

![image-20220915180132070](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915180132070.png)

![image-20220915180030068](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915180030068.png)

【2】更改工作区中Test2.txt中的内容增加bbb

![image-20220915180210841](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915180210841.png)

导致：工作区和暂存区内容不一致，比对：

![image-20220915180701501](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915180701501.png)

总结：git diff [文件名] --》将工作区中的文件和暂存区中文件进行比较

### git diff 

【1】在Test1.txt中添加qqq



![image-20220915180926697](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915180926697.png)

【2】工作区与暂存区的多个文件比对：

![image-20220915181325967](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915181325967.png)

总结：git diff -->比较工作区和暂存区中所有文件的差异

【3】暂存区和本地库的比对：

1.先把工作区更新的文件提交到暂存区：

![image-20220915182046566](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915182046566.png)

2.查看历史版本记录：

![image-20220915182818075](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915182818075.png)

此时本地库HEAD版本与暂存区比对：

![image-20220915183021942](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915183021942.png)

再将暂存区的文件提交到本地库：此时暂存区和本地区文件同步

![image-20220915183229065](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915183229065.png)

![image-20220915183348109](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915183348109.png)

此时修改Test2.txt文件为a：

![image-20220915183444356](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915183444356.png)

在将其添加到暂存区：

![image-20220915183533922](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915183533922.png)

此时可和之前存有aaaaabbb的Test2.txt版本的文件比较也可以和未存有任何值的Test2.txt版本比较：

git diff [版本索引] [文件名]

只需要修改到对应的版本进行比较即可

![image-20220915183853128](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915183853128.png)

![image-20220915183818279](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915183818279.png)

## 10.分支

### 【1】什么是分支：

在版本控制过程中，使用多条线同时推进多个任务。这里面说的多条线，就是多个分支。

### 【2】通过图展示分支：

![image-20220915203015443](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915203015443.png)

### 【3】分支的好处：

同时多个分支可以并发开发，互相不耽误，互相不影响，提高开发的效率

如果有一个分支功能开发失败，直接删除这个分支就可以了，不会对其他分支产生任何影响。

### 【4】分支操作

#### 【1】在工作区创建一个Test5.txt文件，然后提交到暂存区，提交到本地库

![image-20220915204853153](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915204853153.png)

![image-20220915211911244](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915211911244.png)

#### 【2】查看分支（git branch -v）：

![image-20220915212012543](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915212012543.png)

#### 【3】创建分支（git branch [分支名]）

![image-20220915212102560](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915212102560.png)

再查看：

![image-20220915212254730](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915212254730.png)

#### 【4】切换分支（git checkout [分支名]）：

![image-20220915212631779](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915212631779.png)

#### 【5】分支冲突及解决方法

【1】进入branch01分支，增加内容

![image-20220915223251663](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915223251663.png)

![image-20220915223218606](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915223218606.png)

【2】再将分支切换到主分支master

![image-20220915223505306](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915223505306.png)

查看文件Test5.txt,发现为未修改前的文件

![image-20220915223601933](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915223601933.png)

在主分支master下，修改Test5.txt,加入内容

![image-20220915223953432](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915223953432.png)

![image-20220915223911130](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915223911130.png)

【3】再次切换到branch01分支查看：查看文件内容（cat [文件名]）

![image-20220915224508498](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915224508498.png)

【4】将branch01分支合并到主分支：

（1）进入主分支

![image-20220915224809274](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915224809274.png)

（2）将branch01中的内容和主分支内容进行合并：

![image-20220915225534195](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915225534195.png)

查看文件：出现冲突

什么时候会出现冲突？在同一个文件的同一个位置修改

![image-20220915230059619](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915230059619.png)

解决：

公司内部商议解决，或者自己解决，认为设定，留下想要的即可：

![image-20220915230608166](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915230608166.png)

将工作区内容添加到暂存区：

![image-20220915230918917](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915230918917.png)

然后进行commit操作：

![image-20220915231246856](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220915231246856.png)

## 10.远程库

![image-20220916170816696](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916170816696.png)

【1】初始化本地库

![image-20220916164538652](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916164538652.png)

【2】github上新建一个远程库

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916165156454.png" alt="image-20220916165156454" style="zoom:50%;" />

【3】完成状态：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916165254888.png" alt="image-20220916165254888" style="zoom:50%;" />

远程库地址：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916165525938.png" alt="image-20220916165525938" style="zoom:80%;" />

点击进去：

![image-20220916165639297](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916165639297.png)

远程库地址比较长，每次复制比较麻烦

https://github.com/MasterJing66/GitResp02.git

在Git本地将地址保存，通过别名

查看别名：（git remote -v）,如图所示没有任何别名

![image-20220916165929303](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916165929303.png)

远程库地址起别名：git remote add 【别名】 【远程库ip】

![image-20220916170249282](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916170249282.png)

### 推送操作：

![image-20220916171619341](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916171619341.png)

推送后查看远程库：

![image-20220916171838880](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916171838880.png)

### 克隆操作：

远程库地址复制：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916172134717.png" alt="image-20220916172134717" style="zoom:50%;" />

克隆：git clone 【远程库地址】

![image-20220916172444429](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916172444429.png)

克隆操作可以帮我们完成：

（1）初始化本地库

（2）将远程库内容完整的克隆到本地库

（3）替我们创建远程库的别名

![image-20220916172827952](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916172827952.png)

在克隆的文件里新增：

![image-20220916173404978](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916173404978.png)

![image-20220916173351672](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916173351672.png)

【1】更新本地库信息：

![image-20220916173840445](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916173840445.png)

![image-20220916173431670](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916173431670.png)

【2】将更新的内容push到远程库中去

发现可以直接push进去，并没有让我录入账号密码，或者也没提示错误--》结果 很诡异（按理说应该有加入团队的验证，才能向远程库推送文件）

原因：git使用的时候在本地有缓存（git根据本地缓存默认登入）

将缓存删除：

![image-20220916174338768](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916174338768.png)

必须要加入团队：

登录项目经历的账号，邀请普通成员：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916180120353.png" alt="image-20220916180120353" style="zoom:50%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916180327689.png" alt="image-20220916180327689" style="zoom:50%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916180426740.png" alt="image-20220916180426740" style="zoom:50%;" />

登录被邀请者的账号，接受邀请：（在地址栏录入邀请连接即可：http://github.com/zhaoshanshan3366/GitResp2/invitations）

![image-20220916180519110](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916180519110.png)

### 远程库被修改的拉取操作：

【1】拉取操作pull操作，相当于fetch+merge

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916182600805.png" alt="image-20220916182600805" style="zoom: 67%;" />

【2】项目经理先确认远程库内容是否更新了：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916183153900.png" alt="image-20220916183153900" style="zoom: 67%;" />

【3】项目经理进行拉取操作：

（1）先是抓取操作：fetch:

![image-20220916183452109](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916183452109.png)

在抓取操作执行后，只是将远程库的内容下载到本地，但是工作区中的文件并没有更新。工作区中还是原先的内容。

![image-20220916183642104](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916183642104.png)

抓取后可以去远程库看看内容是否正确：

![image-20220916183900673](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916183900673.png)

![image-20220916184006950](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916184006950.png)

然后发现内容都正确，就可以进行合并操作：

（2）进行合并：merge

切换回当前主分支进行合并：

![image-20220916184239049](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916184239049.png)

![image-20220916184257928](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916184257928.png)

远程库的拉取可以直接利用pull命令来完成（git pull ）：

![image-20220916214809449](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916214809449.png)

fetch+merge操作：---》为了保险，慎重，先fetch抓取是为了方便来查看是否满意，避免错误带来的影响

pull--->代码简单，省事

### 协同开发合作时冲突的解决办法

【1】用户：![image-20220916221231824](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916221231824.png)

创建了Tset.txt文件，向远程库推送数据：

![image-20220916222643149](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916222643149.png)

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916221159067.png" alt="image-20220916221159067" style="zoom: 80%;" />

【2】用户：![image-20220916221324248](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916221324248.png)

做了一个拉取操作：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916221338502.png" alt="image-20220916221338502" style="zoom:67%;" />

到这里为止，现在远程合作没有任何问题。

现在操作同一个文件的同一个位置的时候，就会引起冲突：

【3】![image-20220916221631119](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916221631119.png)

再次做了推送操作：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916221622493.png" alt="image-20220916221622493" style="zoom:67%;" />

改动位置：

![image-20220916221711616](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916221711616.png)

【4】用户：![image-20220916223059995](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916223059995.png)

改动Test.txt中的内容，然后进行推送：

![image-20220916221814965](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916221814965.png)

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916221829461.png" alt="image-20220916221829461" style="zoom:67%;" />

发现推送失败！！

在冲突的情况下，先应该拉取下来，然后修改冲突，然后再推送到远程服务器：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916222021450.png" alt="image-20220916222021450" style="zoom:67%;" />

查看冲突：

![image-20220916222124782](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916222124782.png)

认为解决这个冲突（该删则删，该留则留）：

![image-20220916222222614](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916222222614.png)

解决完冲突以后，向服务器推送：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916222320498.png" alt="image-20220916222320498" style="zoom:67%;" />

推送：

![image-20220916222414766](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916222414766.png)

解决了冲突问题：

![image-20220916222355892](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916222355892.png)

## 11.跨团队合作

![image-20220916223800564](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916223800564.png)

### 【1】得到远程库的地址：![image-20220916224038479](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916224038479.png)

![image-20220916224051373](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220916224051373.png)

地址：http://github.com/zhaoshanshan3366/GitResp2.git

### 【2】进行fork操作:<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917192142730.png" alt="image-20220917192142730" style="zoom:67%;" />

进入到账号后：复制地址：http://github.com/zhaoshanshan3366/GitResp2.git

然后点击下面的fork操作：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917192357157.png" alt="image-20220917192357157" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917192609457.png" alt="image-20220917192609457" style="zoom:67%;" />

### 【3】然后就可以克隆到本地，并且进行修改：<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917192941367.png" alt="image-20220917192941367" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917192953344.png" alt="image-20220917192953344" style="zoom:67%;" />

然后更改数据：添加到暂存区，然后提交到本地库，然后push到远程库：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917193637273.png" alt="image-20220917193637273" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917193527311.png" alt="image-20220917193527311" style="zoom:67%;" />

### 【4】进行pull request操作：<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917193839334.png" alt="image-20220917193839334" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917194022591.png" alt="image-20220917194022591" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917194109783.png" alt="image-20220917194109783" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917194445583.png" alt="image-20220917194445583" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917194533231.png" alt="image-20220917194533231" style="zoom:67%;" />

### 【5】进行审核操作：![image-20220917194730744](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917194730744.png)

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917194632859.png" alt="image-20220917194632859" style="zoom:80%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917194817079.png" alt="image-20220917194817079" style="zoom:67%;" />



![image-20220917194838387](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917194838387.png)

可以互相留言：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917194943125.png" alt="image-20220917194943125" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917195005976.png" alt="image-20220917195005976" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917195027652.png" alt="image-20220917195027652" style="zoom:67%;" />

### 【6】查看具体提交的文件确定无误后，进行合并：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917195143020.png" alt="image-20220917195143020" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917195209234.png" alt="image-20220917195209234" style="zoom:67%;" />

### 【7】最后查看库中合并的文件：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917195314319.png" alt="image-20220917195314319" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917195420877.png" alt="image-20220917195420877" style="zoom:67%;" />

## 12.SSH免密登录

免密操作	：

### 【1】进入用户的主目录中：

![image-20220917223138728](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917223138728.png)

### 【2】执行命令，生成一个.ssh的目录中：

![image-20220917223821274](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917223821274.png)

ssh-keygen -t rsa -C 【邮箱】

keygen --->全名（key generation）

注意：C要大写

后面的邮箱，是你的github注册账号的时候对应的邮箱

三次回车确认默认值即可

![image-20220917223757514](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917223757514.png)

发现在ssh目录下有两个文件：

![image-20220917223911593](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917223911593.png)

![image-20220917223921313](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220917223921313.png)

### 【3】打开id_rad.pub文件，将里面的内容进行复制操作：

ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQDHPCQkeJOEuGUCZIxqp6NXLMsG88PjT2omc55wMrpOM/b7eEa/MNjGI1onSngHSLK8gzLRfoJ6VfQSZQGtNdT26ui7IS+V7STVuSrOf1RdqVbk35V8iRWNAaVLElBAmVh+eqQMlyKWFejG8fDMvBdp0Ir67a2s/7TzCPhwzgdK7qi05/pd+B1TO1KOvIvKJhOK5zsJl/KBvu9k7ZQ3k5q4G0AU/36TY834jbzflOJcvXligPRVg3Pr4AdbYmVjeSCoudQ3is0L46qYXB5GRKmBHODx0QQAHxV7lmwzS8w7btSlonSWiYOAXq3Nvq8+4YOQtcKdQJIBFzL2E3A5Ah1/JRCzxczYfUmiskWBB6kr8ScxFNJcARID0X/CEYyb/84TrSFzu9nXlm+2crmRPZVpF1O/XnUkLNnGv+Kwt1qV67Zh8Q55KU80sq6Xp4gkcrz82oObfTj5tklTVsUKyIjDYTRNCkf4z1REWDhLYx7zbTP52U5LrSrvgQJFvCubz2s= 2997132494@qq.com

### 【4】打开github账号

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918195831821.png" alt="image-20220918195831821" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918195947064.png" alt="image-20220918195947064" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918200224005.png" alt="image-20220918200224005" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918200330165.png" alt="image-20220918200330165" style="zoom:67%;" />

### 【5】生成密钥以后，就可以正常进行push操作了：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918200640893.png" alt="image-20220918200640893" style="zoom:67%;" />

对ssh远程地址起别名：

![image-20220918203207498](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918203207498.png)

查看别名：

![image-20220918203241591](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918203241591.png)

创建一个文件：<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918203349803.png" alt="image-20220918203349803" style="zoom:67%;" />

添加到暂存区，提交到本地库：

![image-20220918203840645](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918203840645.png)

第一次push操作，录入yes再回车，才能向远程仓库推送：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918203941346.png" alt="image-20220918203941346" style="zoom: 80%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918204106793.png" alt="image-20220918204106793" style="zoom:67%;" />

ssh方式好处：不用每次都进行身份验证

缺陷：只能针对一个账号

## 13.IDEA集成Git

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918210936094.png" alt="image-20220918210936094" style="zoom: 67%;" />

本地库的初始化操作：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918211242076.png" alt="image-20220918211242076" style="zoom:80%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918211327503.png" alt="image-20220918211327503" style="zoom: 67%;" />

本地库初始化完成了，生成了.git目录：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918211403301.png" alt="image-20220918211403301" style="zoom:80%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918211951493.png" alt="image-20220918211951493" style="zoom:80%;" />

模块也添加到暂存区：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918212143788.png" alt="image-20220918212143788" style="zoom:80%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918212401178.png" alt="image-20220918212401178" style="zoom: 80%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918212518651.png" alt="image-20220918212518651" style="zoom:80%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918212740145.png" alt="image-20220918212740145" style="zoom:80%;" />

当你更改内容以后，前面跟本地库内容不一致的地方会显示绿色：

![image-20220918213348207](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918213348207.png)

## 14.IDEA本地库和远程库的交互

因为他们是两个不同的项目，要把两个不同的项目合并，git需要添加一句代码，**git pull**在之后，这句代码是在git 2.9.2版本发生的，最新的版本需要添加 **--allow-unrelated-histories**告诉git允许不相关的历史合并。							

假如我们的源是origin,分支是master，那么我们需要这样写，**git pull master --allow-unrelated-histories**,这个方法只是解决因为两个仓库有不同的开始点，也就是两个仓库没有共同的commit出现的无法提交。如果使用本文的方法还无法提交，需要看一下是不是发生了冲突，解决冲突再提交

push推送：**git push -u origin master -f**

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918221758964.png" alt="image-20220918221758964" style="zoom:80%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918221649139.png" alt="image-20220918221649139" style="zoom:80%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918221910454.png" alt="image-20220918221910454" style="zoom:80%;" />



到这里远程库和本地库就可以进行交互了

在IDEA中新建一个Person类，并且进行add和commit操作

![image-20220918222207761](C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918222207761.png)

此时在IDEA中进行push操作进行推送

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918222156390.png" alt="image-20220918222156390" style="zoom:80%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918222431455.png" alt="image-20220918222431455" style="zoom:80%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918222540274.png" alt="image-20220918222540274" style="zoom:80%;" />

也可以commit和push一键完成：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918222722209.png" alt="image-20220918222722209" style="zoom:80%;" />

一般在开发先pull操作（防止冲突），再push操作，不会直接进行push操作！！

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918222957120.png" alt="image-20220918222957120" style="zoom:80%;" />

## 15.使用IDEA克隆远程库到本地

利用IDEA进行克隆项目：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918225940705.png" alt="image-20220918225940705" style="zoom:80%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918230315297.png" alt="image-20220918230315297" style="zoom:80%;" />

克隆到本地后：

这个目录既变成了一个本地仓库，有变成了工作空间

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918230639727.png" alt="image-20220918230639727" style="zoom:80%;" />

## 16.使用IDEA解决冲突

【1】在你push以后，有冲突的时候提示合并操作：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918231150893.png" alt="image-20220918231150893" style="zoom:80%;" />

合并：

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918231431206.png" alt="image-20220918231431206" style="zoom: 67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918231636956.png" alt="image-20220918231636956" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918231655571.png" alt="image-20220918231655571" style="zoom:67%;" />

<img src="C:\Users\24687\AppData\Roaming\Typora\typora-user-images\image-20220918231715702.png" alt="image-20220918231715702" style="zoom:80%;" />

## 17.如何避免冲突

【1】团队开发的时候避免在一个文件中改代码

【2】在修改一个文件前，在push之前，先pull操作
