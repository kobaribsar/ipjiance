# Evoxt 日本大阪 Premium Network VPS 深度评测与性能测试

## 产品概览

本次测试机型为 Evoxt 日本大阪 Premium Network VPS，具体配置如下：

- **基础配置**：1核 vCPU / 512MB 内存 / 5GB SSD 存储
- **网络流量**：250GB 月流量
- **价格**：2.99 美元/月（约合人民币 21.5 元）
- **网络线路**：Premium Network（上游为 xTom，回程软银线路）

👉 [【点击查看】2025年最新 Evoxt优惠码及特价云服务器方案汇总](https://bit.ly/evoxt)

## 硬件性能测试

### 系统信息

text
CPU Model Name:        AMD EPYC-Genoa Processor
CPU Cache Size:        L1: 32.00 KB / L2: 1.00 MB / L3: 32.00 MB
Memory Usage:          79.59 MiB / 460.47 MiB
Disk Usage:            2.03 GiB / 4.83 GiB
OS Release:            Debian GNU/Linux 12 (bookworm)
Kernel Version:        6.12.13-x64v3-xanmod1

### CPU 性能

text
1 Thread(s) Test:      5495.74 Scores (1.00x)

### 磁盘 I/O 性能

text
Write Test (4K-Block):   235.85 MB/s (60377 IOPS)
Read Test (4K-Block):    362.32 MB/s (92753 IOPS)
Write Test (128K-Block): 3225.81 MB/s (25806 IOPS)
Read Test (128K-Block):  5263.16 MB/s (42105 IOPS)

## 网络性能测试

### Speedtest 测速结果

| 服务器位置       | 下载速度 | 上传速度 | 延迟 |
|------------------|----------|----------|------|
| xTom - 大阪      | 810 Mbps | 498 Mbps | 16ms |
| 中国移动 - 福建  | 406 Mbps | 7.5 Mbps | 198ms |
| 中国联通 - 上海  | 576 Mbps | 700 Mbps | 57ms |
| 中国电信 - 江苏  | 544 Mbps | 807 Mbps | 38ms |

### 全球 iperf3 测试

**IPv4 测试结果：**
- 新加坡 Leaseweb：753 Mbps 下载 / 503 Mbps 上传
- 洛杉矶 Clouvider：657 Mbps 下载 / 374 Mbps 上传
- 纽约 Leaseweb：591 Mbps 下载 / 585 Mbps 上传

**IPv6 测试结果：**
- 新加坡 Leaseweb：597 Mbps 下载 / 347 Mbps 上传
- 洛杉矶 Clouvider：638 Mbps 下载 / 374 Mbps 上传

## 流媒体解锁测试

### IPv4 解锁情况

- **国际流媒体**：
  - Netflix：支持（日本区）
  - Disney+：支持（日本区）
  - Amazon Prime Video：支持（日本区）
  
- **日本本地服务**：
  - DMM：支持
  - Niconico：支持
  - TVer：支持
  - Radiko：支持（东京地区）

### IPv6 解锁情况

- Netflix：支持（日本区）
- YouTube Premium：支持（日本区）
- Telasa：支持

## 网络路由分析

### 中国电信回程

text
1  Evoxt (大阪) → 2 xTom (大阪) → 3 SoftBank (大阪) 
→ 4 中国电信上海入口 → 5 北京节点
全程延迟：57ms

### 中国联通回程

text
1 Evoxt (大阪) → 2 xTom (大阪) → 3 SoftBank (大阪)
→ 4 中国联通北京入口 → 5 上海节点
全程延迟：59ms

### 中国移动回程

text
1 Evoxt (大阪) → 2 xTom (大阪) → 3 SoftBank (东京)
→ 4 中国移动上海入口
全程延迟：70ms

## 总结评价

Evoxt 日本大阪 VPS 采用 AMD EPYC-Genoa 处理器，性能表现出色，特别适合需要日本节点的用户。主要优势包括：

1. **高性价比**：2.99美元/月的价格极具竞争力
2. **优质网络**：软银回程线路，中国方向延迟低
3. **全面解锁**：支持 Netflix 等主流流媒体日本区
4. **稳定性能**：磁盘 I/O 和网络吞吐量表现优异

适合用途：跨境电商、日本游戏加速、流媒体解锁、企业海外节点等。

👉 [立即获取 Evoxt 日本大阪 VPS 特惠方案](https://bit.ly/evoxt)