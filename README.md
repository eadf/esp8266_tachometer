# esp8266_tachometer
A simple tachometer implementation. This used to be a sub-module in [another project](https://github.com/eadf/esp8266_digoleserial)

It works by seetting up a periodic timer and an interrupt. 
The interrupt increases a counter each time the GPIO alters state. 
The timer calculates the number of alternations over time and presents the frequency [Hz] to the 'clients'.
