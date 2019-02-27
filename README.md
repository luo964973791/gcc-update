-------------------------------------------------
# GCC 4.4.7 升级 GCC 4.8.2  
cd /etc/yum.repos.d && wget http://people.centos.org/tru/devtools-2/devtools-2.repo  
# yum 安装  
yum install devtoolset-2-gcc devtoolset-2-binutils devtoolset-2-gcc-c++  
# 备份
mv /usr/bin/gcc /usr/bin/gcc-4.4.7
mv /usr/bin/g++ /usr/bin/g++-4.4.7
mv /usr/bin/c++ /usr/bin/c++-4.4.7
ln -s /opt/rh/devtoolset-2/root/usr/bin/gcc /usr/bin/gcc
ln -s /opt/rh/devtoolset-2/root/usr/bin/c++ /usr/bin/c++
ln -s /opt/rh/devtoolset-2/root/usr/bin/g++ /usr/bin/g++
