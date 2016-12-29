#1、目的
用命令行来实现对文件夹和文档的操作。
# 2、平台
终端，windows系统上直接用gitbash。
# 3、下面用图文实例的方式，来学习常用命令行以及vim的使用
##3.1  常用Linux命令行，例：对文件夹task2，用git bash打开，测试一下常用命令：
- pwd    查看当前完整路径；

- ls    查看当前目录下文件（不包括隐藏文件）；
- ls -a    查看当前目录下所有文件（包括隐藏文件）；

- ls -al    看当前目录下所有文件（包括隐藏文件）的详细信息；

- cd    切换目录；

- cd ../    回到上级目录；

- touch    新建文件；

- rm    删除文件；

- rm -r    删除文件夹；

- rm -rf    强制删除文件夹；

- mv    重命名；

- mkdir    创建文件夹；

![1.png](http://upload-images.jianshu.io/upload_images/4154091-a8174fab279b6d31.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![2.png](http://upload-images.jianshu.io/upload_images/4154091-03b717d5df914b1b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
##3.2  vim文本编辑工具

可以建立、修改文本文件；在终端下，以命令行的形式实现编辑功能。
主要用途：在被编辑的文件中移动光标的位置，然后方便进行剪切、粘贴、删除、插入、修改等操作。
（1） 在终端，创建或打开文件，命令行如下：
vim *filename*（*filename*为文件名，若文件不存在，则建立一个新文件；若文件存在，则为打开文件）。在终端创建test.html文件，如下：

![3.png](http://upload-images.jianshu.io/upload_images/4154091-41e4077b27815252.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

 （2）常用两种操作模式：命令模式、编辑模式。
 - vim打开默认状态下是命令模式，点击i键，进入编辑模式，状态栏变为Insert

 ![4.png](http://upload-images.jianshu.io/upload_images/4154091-3a5fb6d9d5f86d61.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
 - 按Esc键，退出编辑状态，进入命令状态

 ![5.png](http://upload-images.jianshu.io/upload_images/4154091-6881b6de8d9d0c95.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
 - 保存、退出(在命令模式下进行)
 :w   保存  

  :q    退出(在未作修改的情况下退出)

   :q!    放弃所有修改，直接退出  

     :wq    先保存后退出  （在英文状态下输入）

     ![6.png](http://upload-images.jianshu.io/upload_images/4154091-b168d68e29effa70.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
     - 验证：用Sublime打开在文件test.html

     ![7.png](http://upload-images.jianshu.io/upload_images/4154091-5a6423de37e79ed6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
     （3）常见的文本操作（在命令模式下完成）
     - 快速定位到当前段落开头    ^
     - 快速定位到当前段落结尾    $
      -复制一段文本，并粘贴
              复制：
                    yy复制当前行到内存缓冲区
                     nyy复制N行内容到内存缓冲区
                      y$从光标当前位置复制到行尾
                粘贴：
                      p在光标之后粘贴
                      P在光标之前粘贴
      - 删除几行
                   ndd删除（剪切）n行内容，并去除空隙
      - 快速翻页
                     Ctrl+f下翻一屏 ；Ctrl+d下翻半屏
                     Ctrl+b上翻一屏 ；Ctrl+u上翻半屏
      - 查找某个字符串
                     /learning    正向搜索字符串*learning*
                    ?learning    反向搜索字符串*learning*
