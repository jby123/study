# netty
## IOT字节操作
    ByteBuf buffer = Unpooled.copiedBuffer("123456".getBytes());

    for (int i = 0; i < 3; i++) {
        byte[] data = new byte[2];
        buffer.readBytes(data);
        System.out.println(new String(data));
    }
    
    buffer.resetReaderIndex();//重置指针位置
    
    for (int i = 0; i < 3; i++) {
        byte[] data = new byte[2];
        buffer.readBytes(data);//读取字节数据
        System.out.println(new String(data));
    }
    
    buffer.getCharSequence(1,2, Charset.defaultCharset());//读取字符串