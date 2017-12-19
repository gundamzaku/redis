# redis

用jemalloc方法安装（默认的）  
如果碰到报错，就装jemalloc。还报错  
如果提示“error: jemalloc/jemalloc.h: No such file or directory”，则可以先执行指令：make distclean

make CFLAGS="-g -O0" 关闭优化  

报错：
搜索后分别进入redis下的deps下的hiredis、lua和jemalloc下运行make。  
jemalloc下可能要先运行./configure，然后make。最后回到redis的src下，运行make，出现了一些乱其八糟的东西。  

**make test无法通过**  
安装tcl，还碰到问题，确认which命令是否安装。  

