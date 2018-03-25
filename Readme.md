PHP7-Lua-Install-Script
====

#### Version:
- [Lua](https://www.lua.org/) 5.3.4
- [Pecl-Lua](https://pecl.php.net/package/lua/2.0.5) 2.0.5

#### Requirement:
* php7-dev
* php-pear
* libreadline-dev
* libncurses-dev
* make

How to use on Linux:
```bash
 $ cd /tmp
 $ git clone https://github.com/Raulnet/php7-lua-install-script.git 
 $ cd /
 $ sudo chmod +x /tmp/php7-lua-install-script/install.sh
 $ sudo /tmp/php7-lua-install-script/install.sh
 $ sudo rm -rf /tmp/php7-lua-install-script
```

How to use on Dockerfile:
```dockerfile
FROM php:7.2-apache
...
RUN cd /tmp \
  && git clone https://github.com/Raulnet/php7-lua-install-script.git
RUN ["chmod", "+x", "/tmp/php7-lua-install-script/install.sh"]
RUN /tmp/php7-lua-install-script/install.sh \
  && rm -rf /tmp/php7-lua-install-script
```

