# xLua库集成与编译

[官方参考文档](https://github.com/Tencent/xLua/blob/master/Assets/XLua/Doc/XLua增加删除第三方lua库.md)

## 【集成以下库】
* lua-protobuf

* LuaSocket

* RapidJson

* LPeg


## 【编译】

这里提供能够编译成功的环境配置：

### Windows

1、下载并安装 [Visual Studio 2019](https://visualstudio.microsoft.com/zh-hans/vs/)

2、下载并安装 [CMake 3.19.5](https://cmake.org/download/)

3、把CMake安装目录添加到PATH环境变量，例如 C:\Program Files\CMake\bin

4、编译xlua，例如 make_win32_lua53.bat、make_win64_lua53.bat


### Android

1、下载并安装 [CentOS 7.2 x64](https://www.centos.org/download/)

2、升级gcc/g++到9

3、下载 [CMake 3.19.5](https://cmake.org/download/) 二进制压缩包，解压到指定目录，如/home/cmake

4、下载 [Android NDK r21](https://developer.android.google.cn/ndk/downloads/)，解压到指定目录，如/home/android-ndk

5、vi ~/.bashrc

6、最后一行添加：export PATH=$PATH:/home/cmake/bin

7、最后一行添加：export ANDROID_NDK=/home/android-ndk

8、source ~/.bashrc，让设置生效

9、编译xlua(sh make_android_lua53.sh)


### iOS/MAC

1、下载 [CMake 3.19.5](https://cmake.org/download/) 安装包，安装到Application目录

2、vi ~/.bash_profile 

3、在最后一行添加CMake程序路径：export PATH=/Applications/CMake.app/Contents/bin:$PATH

4、source ~/.bashrc，让设置生效

5、编译xlua，例如 make_ios_lua53.sh、make_mac_lua53.sh
