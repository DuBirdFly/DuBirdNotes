### git
你需要VPN或者DevSidecar
https://www.bilibili.com/video/BV1ua41167Ma
https://www.runoob.com/git/git-workflow.html
(Right click)  git bush here                        //在此处打开git shell
// 注意,用tab键可以自动补全代码


(Type on Git)  git config --global user.name 'DuBirdFly'
(Type on Git)  git config --global user.email '2937823748@qq.com'
(Type on Git)  git clone 'https://github.com/DuBirdFly/tinyRISCV_Learn.git'
// 然后你就会把上面的项目下载下来,这下你在桌面上就有一个'tinyRISCV_Learn'的文件夹
// 然后你用vscode打开这个文件夹,就可以在里面"增删改查"文件夹/文件了,而且vscode是默认关联git的


(Type on Git)  cd tinyRISCV_Learn/                
// 这个时候进入到'tinyRISCV_Learn'这个文件夹
(Type on Git)  git add top.v                      
// workspace(工作区) --> staging area(暂存区/缓存区)
// vscode"源代码管理"处的'+'按钮能实现同'git add'的操作
(Type on Git)  git commit top.v -m '这是一次提交'   
// staging area(暂存区/缓存区) AND workspace(工作区) --> local repository(版本库或本地仓库)
// 不论此时的'top.v'是什么状态,都会被提交到local repository(版本库或本地仓库)
(Type on Git)  git commit -m '全部提交'            
// 单独'git commit'的话,"源代码管理"处的所有代码就会全被提交到local repository(版本库或本地仓库)

(Type on Git)  git push
// local repository(版本库或本地仓库) --> remote repository(远程仓库)

(Type on Git)  git pull
// remote repository(远程仓库) --> workspace(工作区)  ;  更新本地工程

(Type on Git)  git checkout
// 这属于"Git 分支管理"的内容,我反正属实是没看懂



// 包含强调项(但是没有错误)的解决办法,这是一个vscode显示的bug
解决办法:  ctrl+shift+p 输入 (Developer: )reload window
详见 https://stackoverflow.com/questions/59366833/vs-code-containes-emphasized-items-but-no-error


如何将clone下来的项目上传到自己的仓库
https://blog.csdn.net/m0_55546349/article/details/121786789
将clone下来的项目上传到自己的仓库：


//////////////////////////////////////////////////////////////////
https://blog.csdn.net/m0_55546349/article/details/121786789
https://www.cnblogs.com/yinyuxing/p/15840508.html
https://www.runoob.com/git/git-create-repository.html
