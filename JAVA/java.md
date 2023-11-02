# 编码
## ASCII 码
    byte data = 0x65;
    String.format("simCardNo: %c", data) // A 十六进制转字符串
## BCD 码
    String.format("%02d", 0x0A)//10 十六进制转十进制
    String.format("%02X", 10)//0A 十进制转十六进制
## BIN 码
    Long.toBinaryString(0xff)//11111111 十六进制转二进制
    Integer.toHexString(Integer.parseInt("11111111",2)) //ff 二进制转十六进制
## 补0
    String.format("%040d", 65)
## 字节数组转十进制
    byte[] byteArray = {0x01,0x23,0x78,0x12,0x14,0x01,0x32}; // 一个示例字节数组
    BigInteger bigInteger = new BigInteger(1, byteArray); // 使用字节数组创建BigInteger
    long decimalValue = bigInteger.longValue();
    System.out.println(decimalValue);//320473583059250
## String.format()
    String.format("字符串类型 %s",10) //字符串类型 10
    String.format("布尔类型 %b",10) //布尔类型 true
    String.format("整数类型(十进制) %04d",10) //整数类型(十进制) 0010
    String.format("整数类型(十六进制) %04X",10) //整数类型(十六进制) 000A
    String.format("整数类型(八进制) %04o",10) //整数类型(八进制) 0012
    String.format("浮点类型 %.3f",7.7) //浮点类型 7.700
    String.format("十六进制浮点类型 %.1a",254.4) //十六进制浮点类型 0x1.0p8
    String.format("散列码 %h",1010) //散列码 3f2
    String.format("百分比类型 %d%%",10) //百分比类型 10%
    String.format("字母A的散列码是：%h",'1') //字母A的散列码是：31
    String.format("上面价格的指数和浮点数结果的长度较短的是：%.3g", 2 * 0.85) //上面价格的指数和浮点数结果的长度较短的是：1.70
    String.format("%tF %tT", new Date(), new Date()) //2023-10-17 15:05:20
    String.format("%tF %tT", System.currentTimeMillis(), System.currentTimeMillis()) //2023-10-17 15:05:20

# 位运算
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
## &(AND) 逻辑与运算
    1 & 3: 1
    2 & 3: 2
    3 & 3: 3
    4 & 3: 0
    5 & 3: 1
    6 & 3: 2
    7 & 3: 3
    8 & 3: 0
    9 & 3: 1
## |(OR) 逻辑或运算
    1 | 3: 3
    2 | 3: 3
    3 | 3: 3
    4 | 3: 7
    5 | 3: 7
    6 | 3: 7
    7 | 3: 7
    8 | 3: 11
    9 | 3: 11
## % 求余数
    1 % 3: 1
    2 % 3: 2
    3 % 3: 0
    4 % 3: 1
    5 % 3: 2
    6 % 3: 0
    7 % 3: 1
    8 % 3: 2
    9 % 3: 0
        
# 请求框架

## okhttp
## [forest](https://forest.dtflyx.com/)

# 工具
## [hutool](https://www.hutool.cn/)
## [swagger](/demo)
## [knife4j](https://doc.xiaominfo.com/)

# spring boot
## [springboot](/JAVA/springboot.md)

 
## (缓存框架)spring boot cache

# 学习资源
## [未读代码](https://www.wdbyte.com/)
## [JSR](https://openjdk.org/jeps/201)

# 环境安装包
## [graalvm](https://www.graalvm.org/downloads-thanks/)