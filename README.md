eGizmo Ethernet Shield for Arduino Duemilanove ATmega328
========================================================

Additional fix:
* Updated ```enc28j60.c``` for Arduino 1.0
* Fixed include directive in etherShield.cpp

Working in Arduino 1.6.7.

Fixed these errors:

C:\Program Files (x86)\Arduino\libraries\etherShield/ip_arp_udp_tcp.h:32:66: error: 'prog_char' does not name a type
 extern uint16_t fill_tcp_data_p(uint8_t *buf,uint16_t pos, const prog_char *progmem_s);

C:\Program Files (x86)\Arduino\libraries\etherShield/ip_arp_udp_tcp.h:32:77: error: ISO C++ forbids declaration of 'progmem_s' with no type [-fpermissive]
 extern uint16_t fill_tcp_data_p(uint8_t *buf,uint16_t pos, const prog_char *progmem_s);

C:\Program Files (x86)\Arduino\libraries\etherShield/etherShield.h:34:65: error: 'prog_char' does not name a type
    uint16_t ES_fill_tcp_data_p(uint8_t *buf,uint16_t pos, const prog_char *progmem_s);
                                                                
C:\Program Files (x86)\Arduino\libraries\etherShield/etherShield.h:34:76: error: ISO C++ forbids declaration of 'progmem_s' with no type [-fpermissive]
    uint16_t ES_fill_tcp_data_p(uint8_t *buf,uint16_t pos, const prog_char *progmem_s);
