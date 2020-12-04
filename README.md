ffplay 源码调试

环境安装：

推荐使用UOS作为开发环境。且此环境配置是在UOS下完成。

1.打开ffmpeg_study/MyHelp,复制lib_preinstall的文本到命令行执行，

2.若此时还存在ld错误。请检查/usr/下的相应的动态库是否格式为.so形式。若不是，则参照Ln-lib.log文件创建链接相应的.so文件.

编译:
1.  ./configure --enable-static --prefix=./MyBuild --enable-libfreetype --enable-filter=subtitles --enable-libass

2.  make

3.make install

调试：
1.用vscode打开ffmpeg_study
2.打开fftools/ffplay.c
3.并已ffplay.c为目标，点击debugging开始调试

错误：
若还是无法正常使用，请提issues.
