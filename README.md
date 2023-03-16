# Morse-code

## Morse code and seven segment display using 8051 microcontroller and keil uvision software 


**Parts required**

*8051 Microcontroller*

*8051 Development Board like 89V51RD2*


**Theory**

*By activating and deactivating GPIO pins we can give the appropriate Binary code to get the morse code of the character*

*else if(s==0x7c) represents 'B' in binary no. which we manually cofigure on keil uvision, so that we get its morse code equivalent on LED & also characters on 7 segment display*

```
unsigned char code B[]={0x00,0x01,0x01,0x01,0x00,0x01,0x00,0x01,0x00,0x01,0x00} where 0x01 is high for led which represents _ and 0x00 is low which represents a space so
this whole binary no. states "  _...  "  which is 'B' in morse code for 8051 GPIO pins
```

*one(); | two(); | three(); | four(); functions represent Out of which of the 4 seven segment display we chose to display the character*


## Note:
  ***We need to manually change the GPIO pins in the software after step by step execution i.e. while line 53 is run we need to change the pin P3 in the options***
