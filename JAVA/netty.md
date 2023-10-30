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
        log.info("读取数据前指针位置:{}", buffer.readerIndex());
        log.info("引用计数器:{}", buffer.refCnt());
        byte[] data = new byte[2];
        // 读取数据并改变指针
        buffer.readBytes(data);
        log.info("读取数据:{}",new String(data));
    }