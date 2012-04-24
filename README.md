tsar-mod_nginx
==============

nginx module for tsar

###Can be used with nginx and tengine both.

Quick start
-----------
1. Install tsar from http://code.taobao.org/p/tsar/src/.
2. Generate a new module by using tsardevel.
    http://code.taobao.org/p/tsar/wiki/mod/
    #tsardevel ngx_mod
3. Replace ngx_mod.c.
    then,
    #make
    #make install
4. tsar --nginx,be happy with it.

Configuration
-------------
Nginx server port to be monitored,default is 80.
    example: export NGX_TSAR_PORT=8080
