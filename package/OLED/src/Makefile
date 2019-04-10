OLED: ssdtest.o SSD1306.o
	$(CC) $(LDFLAGS) SSD1306.o ssdtest.o -o OLED
SSD1306.o: SSD1306.c SSD1306.h font8x8.h font5x7.h
	$(CC) $(CFLAGS) -c SSD1306.c  
ssdtest.o: ssdtest.c SSD1306.h
	$(CC) $(CFLAGS) -c ssdtest.c
clean: rm *.o OLED
