# Install-UA-Lua
Make UA-Lua script work on CentOS

- Install lua libraries

        # yum install luarocks
        # uarocks install json2lua
        # luarocks install json
        # luarocks install lrexlib-pcre

- Install LuaJIT

        # wget "http://luajit.org/download/LuaJIT-2.0.4.tar.gz"
        # tar xzvf LuaJIT-2.0.4.tar.gz 
        # cd LuaJIT-2.0.4
        # make
        # make install

- Install Nginx with Lua module

        # wget https://github.com/simpl/ngx_devel_kit/archive/master.zip
        # unzip master.zip 
        # rm -f master.zip 
        # wget https://github.com/openresty/lua-nginx-module/archive/master.zip
        # unzip master.zip 
        # rm -f master.zip 
        # export LUAJIT_LIB=/usr/local/lib
        # export LUAJIT_INC=/usr/local/include/luajit-2.0
      
