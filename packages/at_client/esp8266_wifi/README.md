[rtthread - Ӧ�� AT ������� ESP8266 ģ��](https://www.rt-thread.org/document/site/application-note/components/at/an0014-at-client/)
[��������](https://www.rt-thread.org/document/site/rtthread-studio/drivers/uart/v4.0.2/rtthread-studio-uart-v4.0.2/)  


#### ����rtthread
components (���)
Enable AT commands client

packages (�����)
AT DEVICE (AT �豸)
����ESP8266


#### �������� (WIFI - UART2)
board.h
```diff
+ #define BSP_USING_UART2
+ #define BSP_UART2_TX_PIN       "PA2"
+ #define BSP_UART2_RX_PIN       "PA3"
```

#### ����WIFI (SSID, PASSWORD)
rtconfig.h
```
#define ESP8266_SAMPLE_WIFI_SSID "rtthread"
#define ESP8266_SAMPLE_WIFI_PASSWORD "12345678"
```


#### �쳣 - wait AT client(uart2) connect timeout
����:
msh />[E/at.clnt] wait AT client(uart2) connect timeout(5000 tick).
���:
��Ҫ��ESP8266ģ������(��������)(�ֶ����һ��ģ��)


#### ��֤WIFI��������
```
ping 8.8.8.8
32 bytes from 8.8.8.8 icmp_seq=3 time=203 ms
```
