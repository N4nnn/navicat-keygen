# Navicat Keygen - 如何编译？

## 1. 前提条件

1. 请确保你安装了下面几个库：

   * `capstone`
   * `keystone`
   * `rapidjson`
   * `openssl`

   你可以通过下面的命令来安装它们：

   ```console
   # install capstone
   $ sudo apt-get install libcapstone-dev

   # install keystone
   $ sudo apt-get install cmake
   $ git clone https://github.com/keystone-engine/keystone.git #如果慢的话用 https://gitee.com/kite0101/keystone.git
   $ cd keystone
   $ mkdir build
   $ cd build
   $ ../make-share.sh
   $ sudo make install
   $ sudo ldconfig

   # install rapidjson
   $ sudo apt-get install rapidjson-dev

   # install openssl
   $ sudo apt-get install openssl
   ```

2. 你的gcc支持C++17特性。 

## 2. 编译

```console
$ git clone https://github.com/zzzsyyy/navicat-keygen.git
$ cd navicat-keygen
$ make all
```

生成完成后，你会在 `bin/` 文件夹下看到编译后的keygen/patcher。
