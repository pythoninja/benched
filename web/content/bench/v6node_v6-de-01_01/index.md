---
title: "V6node (v6-de-01) Benchmark #01"
date: 2023-05-07T21:28:19+03:00
lastmod: 2023-05-07T21:28:19+03:00
tags:
    - yabs
    - v6node
    - v6-de-01

draft: false
---

## Yabs Output

```text
Fri May  5 16:31:30 UTC 2023

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 9 minutes
Processor  : AMD EPYC 7402 24-Core Processor
CPU cores  : 2 @ 2799.998 MHz
AES-NI     : ✔️ Enabled
VM-x/AMD-V : ✔️ Enabled
RAM        : 3.8 GiB
Swap       : 0.0 KiB
Disk       : 25.0 GiB
Distro     : AlmaLinux 8.7 (Stone Smilodon)
Kernel     : 4.18.0-425.13.1.el8_7.x86_64
VM Type    : KVM
IPv4/IPv6  : ✔️ Online / ✔️ Online

IPv6 Network Information:
---------------------------------
ISP        : Ian David Klemm
ASN        : AS200461 Ian David Klemm
Host       : Ian David Klemm
Location   : Rotterdam, South Holland (ZH)
Country    : Netherlands

fio Disk Speed Tests (Mixed R/W 50/50):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 225.88 MB/s  (56.4k) | 2.64 GB/s    (41.3k)
Write      | 226.47 MB/s  (56.6k) | 2.66 GB/s    (41.5k)
Total      | 452.36 MB/s (113.0k) | 5.30 GB/s    (82.9k)
           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 7.65 GB/s    (14.9k) | 3.01 GB/s     (2.9k)
Write      | 8.05 GB/s    (15.7k) | 3.21 GB/s     (3.1k)
Total      | 15.70 GB/s   (30.6k) | 6.22 GB/s     (6.0k)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping           
-----           | -----                     | ----            | ----            | ----           
Clouvider       | London, UK (10G)          | 3.19 Gbits/sec  | 3.84 Gbits/sec  | 12.6 ms        
Scaleway        | Paris, FR (10G)           | busy            | 4.40 Gbits/sec  | 9.47 ms        
NovoServe       | North Holland, NL (40G)   | busy            | 6.18 Gbits/sec  | 7.20 ms        
Uztelecom       | Tashkent, UZ (10G)        | 1.68 Gbits/sec  | 1.94 Gbits/sec  | 75.7 ms        
Clouvider       | NYC, NY, US (10G)         | 1.71 Gbits/sec  | 194 Mbits/sec   | 82.3 ms        
Clouvider       | Dallas, TX, US (10G)      | 860 Mbits/sec   | 1.36 Gbits/sec  | 115 ms         
Clouvider       | Los Angeles, CA, US (10G) | 1.09 Gbits/sec  | busy            | 139 ms         

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping           
-----           | -----                     | ----            | ----            | ----           
Clouvider       | London, UK (10G)          | 3.71 Gbits/sec  | 2.48 Gbits/sec  | 12.5 ms        
Scaleway        | Paris, FR (10G)           | 3.55 Gbits/sec  | busy            | 12.8 ms        
NovoServe       | North Holland, NL (40G)   | 4.87 Gbits/sec  | 6.57 Gbits/sec  | 7.13 ms        
Uztelecom       | Tashkent, UZ (10G)        | 1.58 Gbits/sec  | busy            | 75.7 ms        
Clouvider       | NYC, NY, US (10G)         | 1.15 Gbits/sec  | busy            | 82.3 ms        
Clouvider       | Dallas, TX, US (10G)      | 26.4 Mbits/sec  | 1.48 Gbits/sec  | 115 ms         
Clouvider       | Los Angeles, CA, US (10G) | 41.0 Mbits/sec  | 294 Mbits/sec   | 139 ms         

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value                         
                |                               
Single Core     | 1336                          
Multi Core      | 2418                          
Full Test       | https://browser.geekbench.com/v6/cpu/1158469
```

Download metrics as text: [yabs.txt](./yabs.txt)
