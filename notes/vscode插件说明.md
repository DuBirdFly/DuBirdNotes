###  通用设置

[vscode与git联合设置](https://www.bilibili.com/video/BV1ua41167Ma)

#### 忽略.bak文件
如果我不想显示".bak"这样的文件可以打开VSCode->setting->text editor->files->exclude->add pattern->
```json
**/*.bak
```

或者按下Ctrl+shift+p搜索settings（json）点击打开填写：
```json
"files.exclude":
{
"**/*.meta": true
}
```

#### 键盘快捷键方式
文件-首选项-键盘快捷方式

#### 字体
文件-首选项-设置（用户区/工作区）-文本编辑器-字体
```json
"editor.fontFamily": "JetBrains Mono",
"editor.fontFamily": "Fira Code",
```

#### tab首选项设置
tabsize    4
Editor: Detect Indentation(是否自动控制tab,一般在接管老程序的时候有用)      true or false

#### 折行
Diff Editor: Word Wrap         // 超出可显示范围时折到下一行,设置wordWrapColumn
vscode 折行起始位置: Editor: Word Wrap Column  // 默认为80,我设置为100

### 通用插件
#### vscode-icons
不同文件夹和文件显示为不同的图标

####  GBKtoUTF8
自动将文件的编码方式由GBK转为UTF8

#### TCL Language Support
约束文件的语法高亮(再也不是一片白了)[我反正也不知道有什么用...]

####  Bracket Pair Colorizer
多重括号显示为不同颜色

#### Gitlens
​使用VSCode的原因之一，便是VSCode官方自带版本管理功能。而Gitlens是对GIT的版本控制的补充。开启Gitlens后，每一行都可以看到提交信息。可以快速的插件代码差异再爽不过了。 

#### Code Alignment
安装好，即可实现的功能：
- 按字符进行代码对齐
- 按正则表达式进行代码对齐

如下图，默认有五种对齐方式，对于我来说，其中的按字符对齐和按正则表达式对齐就足够适应所有的情况。我习惯将对齐的快捷键更改为`Alt+A`;

![按键](https://img-blog.csdnimg.cn/20200409230549999.png#pic_center)
![示例](https://img-blog.csdnimg.cn/20200409230607472.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L05lb2NzdA==,size_16,color_FFFFFF,t_70#pic_center)

#### Tabout
按Tab键跳出引号、括号等

#### rainbow end
相当于支持end的彩虹括号 

#### 中文标点符号转英文
插件名字就叫这个,或者叫autopunc,或者不用这个插件直接在windows设置"中英文标点切换"即可

### Verilog 插件
[尤老师的FPGA插件-视频](https://www.bilibili.com/video/BV1SK4y1S79m)
[尤老师的FPGA插件-PDF](dataDoc/第一讲、VScode编辑器软件安装.pdf)

#### Verilog-HDL
**自行添加自动填充的文件目录**
C:\Users\hp\.vscode\extensions\mshr-h.veriloghdl-1.5.1\snippets\verilog.json
**自动例化**：
Ctrl+shift+P --> (tpye on)verilog --> (choose)System Verilog:Instance Module

#### hexdump for VSCode
可以查看二进制文件(对于FPGA开发查看二进制文件的需求不是很多，但也有。我很少去打开BIN文件，但我经常去比对Zynq器件的HDF文件–)

####  verilog-simplealign
代码格式化：全选-->ctrl+l

####  Verilog_Testbench
生成Testbench内容：ctrl+shift+p -> Testbench


### Markdown插件

#### Markdown All in One
核心插件

#### Markdown Preview Enhanced
更好的markdown可视化

#### Paste Image
复制图片到markdown,注意图片粘贴变成了"ctrl+alt+v"
这个插件实际上就是自动化生成图片模板
