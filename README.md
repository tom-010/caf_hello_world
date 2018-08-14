CAF Hello World
===============

This is a example of a standalone hello world with the C++ Actor Framework: https://github.com/actor-framework

To run it follow the following steps:

1. (Install CAF) cd /tmp/folder/for/caf/files
2. git clone --recursive https://github.com/actor-framework/actor-framework.git
3. cd actor-framework
4. ./configure && make && make test && sudo make install (CAF ist now installed)
5. (Build&Run The example) mkdir build && cd build
6. cmake ..
7. make
8. ./hello_world

This is tested on Ubuntu 18.04
