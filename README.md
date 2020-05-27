### cmake升级

```javascript
#CentOS7升级
yum install epel-release -y
yum remove cmake -y
yum install cmake3 -y
ln -s /usr/bin/cmake3 /usr/bin/cmake
```

### gcc 8.3升级

```javascript
#CentOS7
yum -y install centos-release-scl
yum -y install devtoolset-8-gcc devtoolset-8-gcc-c++ devtoolset-8-binutils
echo "source /opt/rh/devtoolset-8/enable" >>/etc/profile
source /etc/profile
```

