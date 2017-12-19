# redis

用jemalloc方法安装（默认的）  
如果碰到报错，就装jemalloc。还报错  
如果提示“error: jemalloc/jemalloc.h: No such file or directory”，则可以先执行指令：make distclean

make CFLAGS="-g -O0" 关闭优化  
