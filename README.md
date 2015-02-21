# esp8266_tachometer
A simple tachometer implementation. This used to be a sub-module in [another project](https://github.com/eadf/esp8266_digoleserial)

It works by seetting up a periodic timer and an interrupt. 
The interrupt intreases a counter each time GPIO alters state. 
The timer calculates the number of alternations over time and presents that number to the 'clients'.
