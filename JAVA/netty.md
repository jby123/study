# netty
## IOT字节操作
    ByteBuf buffer = Unpooled.copiedBuffer("123456".getBytes());
    
    log.info("字节大小:{}", buffer.capacity());
    
    log.info("读取char 数据:{}", buffer.getCharSequence(0, 5, Charset.defaultCharset()));
    
    for (int i = 0; i < 3; i++) {
        byte[] data = new byte[2];
        buffer.readBytes(data);
        System.out.println(new String(data));
    }
    
    buffer.resetReaderIndex();//重置指针位置 
    
    //判断是否有数据
    while (buffer.isReadable()) {
        log.info("读取数据前指针位置:{} 待读取数据大小:{}", buffer.readerIndex(), buffer.readableBytes());
        log.info("引用计数器:{}", buffer.refCnt());
        byte[] data = new byte[2];
        // 读取数据并改变指针
        buffer.readBytes(data);
        log.info("读取数据:{}",new String(data));
    }
    
## 沾包问题处理
    new DelimiterBasedFrameDecoder(
            1024,
            Unpooled.copiedBuffer("5AA5".getBytes()),
            Unpooled.copiedBuffer("5AA5".getBytes())
    )
## 
    byte： 1字节，8位，有符号
    short：2字节，16位，有符号
    int：  4字节，32位，有符号
    long： 8字节，64位，有符号