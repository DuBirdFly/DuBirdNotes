## 连接上Git
你需要VPN或者[DevSidecar](https://gitee.com/docmirror/dev-sidecar)

## 教学文档
[git与vscode联合使用-视频](https://www.bilibili.com/video/BV1ua41167Ma)
[git教程-网页](https://www.runoob.com/git/git-tutorial.html)

## Git一般流程



### 打开git bush
```git
//打开git shell(用tab键可以自动补全代码)
(右键)  git bush here                        
```

### clone代码
```git
git config --global user.name 'DuBirdFly'
git config --global user.email '2937823748@qq.com'
git clone 'https://github.com/DuBirdFly/tinyRISCV_Learn.git'
```

### clone的项目上传到自己的仓库
[如何将clone下来的项目上传到自己的仓库](https://blog.csdn.net/m0_55546349/article/details/121786789)<br>
```git
git clone 'https://xxx/xxxx/xxxx.git'     // clone你需要的项目
cd xxx                  // 进入项目根目录
rm -r .git              // 删除原有的git信息，有问题一直回车
git init                // 初始化git
git add .               // add当前目录下所有变化的文件
git commit -m “xxx”     // 本地代码添加到仓库
git remote add origin 远程库地址            // 关联远程库,注意远程库不要生成README
git push --set-upstream origin master     // 提交代码
```

### 常用指令

#### cd
```json
// 进入到某一级目录下,如进入到'tinyRISCV_Learn'这个文件夹
(Type on Git)  cd tinyRISCV_Learn/                
```
#### add
```json
// workspace(工作区) --> staging area(暂存区/缓存区)
// vscode"源代码管理"处的'+'按钮能实现同'git add'的操作
(Type on Git)  git add top.v                      
```
注:[git add . 和 git add --all 的区别](https://www.cnblogs.com/yinyuxing/p/15840508.html)

#### commit
```git
git commit top.v -m '这是一次提交'   
// staging area(暂存区/缓存区) AND workspace(工作区) --> local repository(版本库或本地仓库)
// 不论此时的'top.v'是什么状态,都会被提交到local repository(版本库或本地仓库)
```
```git 
git commit -m '全部提交'            
// 单独'git commit'的话,"源代码管理"处的所有代码就会全被提交到local repository(版本库或本地仓库)
```

#### push
```git 
(Type on Git)  git push
// local repository(版本库或本地仓库) --> remote repository(远程仓库)
```

#### pull
```git
(Type on Git)  git pull
// remote repository(远程仓库) --> workspace(工作区)  ;  更新本地工程
```

#### checkout
```git
(Type on Git)  git checkout
// 这属于"Git 分支管理"的内容,我反正属实是没看懂
```

### 常见BUG
#### 包含强调项
// [包含强调项(但是没有错误)的解决办法](https://stackoverflow.com/questions/59366833/vs-code-containes-emphasized-items-but-no-error),这其实是一个vscode显示的bug
解决办法:  ctrl+shift+p 输入 (Developer: )reload window







<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>