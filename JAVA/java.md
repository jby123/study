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
    
# 请求框架

## okhttp
## [forest](https://forest.dtflyx.com/)

# 工具
## [hutool](https://www.hutool.cn/)
## [swagger](/demo)
## [knife4j](https://doc.xiaominfo.com/)

# spring boot
 
## (缓存框架)spring boot cache