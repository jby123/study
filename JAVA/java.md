# 编码
## ASCII 码
    byte data = 0x65;
    String.format("simCardNo: %c", data) // A 十六进制转字符串
## BCD 码
    String.format("%02d", 0x0A)//10 十六进制转十进制
    String.format("%02X", 10)//0A 十进制转十六进制
## BIN 码
    Long.toBinaryString(0xff)//11111111 十六进制转二进制
## 补0
    String.format("%040d", 65)
## 位移
    1 << 3: 8 | 8 >> 3: 1
    2 << 3: 16 | 16 >> 3: 2
    3 << 3: 24 | 24 >> 3: 3
    4 << 3: 32 | 32 >> 3: 4
    5 << 3: 40 | 40 >> 3: 5
    6 << 3: 48 | 48 >> 3: 6
    7 << 3: 56 | 56 >> 3: 7
    8 << 3: 64 | 64 >> 3: 8
    9 << 3: 72 | 78 >> 3: 9
    
## XOR 异或运算
    XOR 1 ^ 3: 2 | 1 ^ 3 ^ 3: 1
    XOR 2 ^ 3: 1 | 2 ^ 3 ^ 3: 2
    XOR 3 ^ 3: 0 | 3 ^ 3 ^ 3: 3
    XOR 4 ^ 3: 7 | 4 ^ 3 ^ 3: 4
    XOR 5 ^ 3: 6 | 5 ^ 3 ^ 3: 5
    XOR 6 ^ 3: 5 | 6 ^ 3 ^ 3: 6
    XOR 7 ^ 3: 4 | 7 ^ 3 ^ 3: 7
    XOR 8 ^ 3: 11 | 8 ^ 3 ^ 3: 8
    XOR 9 ^ 3: 10 | 9 ^ 3 ^ 3: 9
    
# 请求框架

## okhttp
## [forest](https://forest.dtflyx.com/)

# 工具
## [hutool](https://www.hutool.cn/)
## [swagger](/demo)
## [knife4j](https://doc.xiaominfo.com/)

# spring boot
 
## (缓存框架)spring boot cache