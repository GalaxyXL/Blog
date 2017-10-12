title: Ubuntu 16.04 LTS 更换内核安装锐速
date: 2017-10-12 19:38:20
author: 2


---
# Unbuntu 16.04 更换内核安装锐速

## 更换内核

### 安装要求内核
```bash
apt-get install linux-image-4.4.0-47-generic  
apt-get install linux-image-extra-4.4.0-47-generic

apt-get install linux-headers-4.4.0-47  
apt-get install linux-headers-4.4.0-47-generic

```
### 删除以前的内核

#### 查看内核
```bash
dpkg --list | grep image  
dpkg --list | grep headers
```
#### 删除内核
```bash
apt-get purge linux-image-4.4.0-XX-generic  
apt-get purge linux-headers-4.4.0-XX
```
完成上述操作后重启

## 安装锐速
```bash
wget --no-check-certificate -O appex.sh https://raw.githubusercontent.com/0oVicero0/serverSpeeder_Install/master/appex.sh && chmod +x appex.sh && bash appex.sh install
```
