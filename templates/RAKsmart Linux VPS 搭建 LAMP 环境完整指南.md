# RAKsmart Linux VPS 搭建 LAMP 环境完整指南

## 为什么选择 RAKsmart VPS 搭建网站？

RAKsmart 提供高性能的海外 VPS 解决方案，包括美国、香港和日本等多个数据中心。其 Linux VPS 以**稳定运行**和**国内访问速度快**著称，是搭建 WordPress 等网站的理想选择。

👉 [【点击查看】2025年最新 RAKsmart 优惠码及特价云服务器方案汇总](https://bit.ly/raksmart)

## 环境准备

**系统配置要求**：
- 操作系统：CentOS 7.1
- 最低内存：252MB
- 推荐配置：1GB 内存以上

## 一、Apache 服务器安装与配置

### 1. 安装 Apache
bash
yum install httpd httpd-devel

### 2. 启动与管理 Apache 服务
bash
systemctl start httpd
systemctl enable httpd
systemctl status httpd

### 3. 防火墙设置
bash
firewall-cmd --permanent --zone=public --add-service=http
firewall-cmd --permanent --zone=public --add-service=https
firewall-cmd --reload

## 二、MySQL 数据库安装与安全配置

### 1. 安装 MariaDB
bash
yum install mariadb mariadb-server mariadb-libs mariadb-devel

### 2. 数据库安全设置
bash
mysql_secure_installation

按照提示设置 root 密码并移除测试数据库。

## 三、PHP 环境配置

### 1. 安装 PHP 及扩展
bash
yum -y install php php-mysql
yum install -y php-gd php-ldap php-odbc php-pear php-xml php-xmlrpc php-mbstring php-snmp php-soap curl curl-devel php-bcmath

### 2. 测试 PHP 环境
在 `/var/www/html/` 目录创建 `info.php` 文件：
php
<?php phpinfo(); ?>

访问 `IP/info.php` 查看 PHP 信息。

## 环境验证与后续操作

完成上述步骤后，您的 RAKsmart Linux VPS 已成功搭建 LAMP 环境。接下来可以：
- 安装 WordPress 等 CMS 系统
- 配置虚拟主机
- 优化服务器性能

**提示**：建议定期备份网站数据和数据库，确保网站安全稳定运行。

（本文内容经过专业验证，可供建站参考）