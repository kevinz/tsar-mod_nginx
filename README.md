tsar-mod_nginx
==============

#nginx module for tsar

##Can be used with nginx and tengine both.

Quick start
-----------
1. Install [tsar](http://code.taobao.org/p/tsar/src/).
2. Generate a new module by using [tsardevel](http://code.taobao.org/p/tsar/wiki/mod/).
    >`tsardevel ngx_mod`
3. Replace ngx_mod.c.
    >`make`
    >`make install`
4. >`tsar --nginx`

###You should be happy with it.

Configuration
-------------
1. We can change nginx server port to be monitored,default is 80.

    example: 
    >`export NGX_TSAR_PORT=8080`

2. Stub Status module must be included,and add configuration as below:

    >location =  /status {
    >         stub_status on;
    >}
