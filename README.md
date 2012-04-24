tsar-mod_nginx
==============

nginx module for tsar

###Can be used with nginx and tengine both.

Quick start
-----------
1. Install tsar from http://code.taobao.org/p/tsar/src/.
2. Generate a new module by using tsardevel,there is a guide, http://code.taobao.org/p/tsar/wiki/mod/.
    <br/>
    #tsardevel ngx_mod
3. Replace ngx_mod.c.
    then,
    <br/>
    #make
    <br/>
    #make install
4. tsar --nginx,be happy with it.

Configuration
-------------
1. We can change nginx server port to be monitored,default is 80.
    <br/>
    example: export NGX_TSAR_PORT=8080

2. Stub Status module must be included,and add configuration as below:
    <br/>
    location =  /status {
             stub_status on;
    }
