# 概述
## 基本思想
一、一切都是文件
二、每个软件都有确定的用途

## FHS标准 filesystem hierarchy standard
/boot  启动目录，内核存放地  
/ect   配置文件存放地  
/tmp   程序产生的临时文件  
/home  用户目录，新增账户时，用户的家目录存放地  
/lib   库文件  
/bin   可执行文件和常用的Linux命令  
/sbin  系统管理员的命令和工具  
/usr   应用程序和文件安装地  
/mnt   挂接其他文件系统  
/root  root账户的home目录  
/dev   存放Linux系统下的设备文件  

### vi
功能：生成新文件或编辑、查看文件  
格式：vi file_name  
i     插入文本  
a     追加文本  
Esc   从编辑模式进入命令模式  
#### 命令模式
:w - 保存文件  
:wq - 保存并退出  
:wq! - 保存并强制退出  
:q - 退出  
:q! - 强制退出  
dd - 删除一行文字  
x - 删除一个字符  
:n - 光标移至文本第n行  
$ - 光标移至文本的行尾  
G - 光标移至文本的末尾  
/ - 查找某个字符串
  
### pwd (print work directory)
功能：打印用户当前所处的路径  

### cd (change directory)
功能：改变用户所在目录
cd .. - 返回当前目录的上一句目录  
cd - 返回当前用户的主目录  
cd /home 切换到home目录  

### ls (list directory)
功能：显示指定目录下的内容  
ls -a -> 列举目录中的全部文件，包括隐藏文件  
ls -l -> 列举目录中的细节，如权限、所有者、族群、大小、创建日期  
ls -al -> 显示包括隐藏信息在内的所有文件的信息  
ls -r -> 逆向从后向前列举目录的内容  
ls -R -> 递归地列举当前目录下所有子目录的内容  
Is -s -> 文件大小（以数据块为单位）  
ls -l 1.txt -> 列举文件1.txt的所有信息  


### cat (concatenate)
功能：显示文件内容
cat 1.txt  

### touch
功能：创建文本，不能插入内容  
touch 1.txt 2.txt 3.txt  

### grep
功能：在文件中找到特定的字符串  
grep content 1.txt  

### cp (copy)
功能：复制文件  
copy -i -> 如果目标目录有相同文件，会提示是否覆盖  
copy -r -> 复制整个目录、子目录及文件  
copy -v -> 显示文件的复制进度
