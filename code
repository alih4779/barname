/*------------------------------------------------------------------------
  Example sketch for Adafruit Thermal Printer library for Arduino.
  Demonstrates some of the available alternate characters.
  See 'A_printertest' sketch for a more generalized printing example.

  THESE FEATURES ARE NOT AVAILABLE ON ALL PRINTERS.  Older firmware
  does not support the alternate characters used here.
  ------------------------------------------------------------------------*/

#include "Adafruit_Thermal.h"


// Here's the syntax when using SoftwareSerial (e.g. Arduino Uno) --------
// If using hardware serial instead, comment out or remove these lines:

#include "SoftwareSerial.h"
#define TX_PIN 6 // Arduino transmit  YELLOW WIRE  labeled RX on printer
#define RX_PIN 5 // Arduino receive   GREEN WIRE   labeled TX on printer

SoftwareSerial mySerial(RX_PIN, TX_PIN); // Declare SoftwareSerial obj first

SoftwareSerial nSerial(8, 9);  // Declare SoftwareSerial obj first




Adafruit_Thermal printer(&mySerial);     // Pass addr to printer constructor
// Then see setup() function regarding serial & printer begin() calls.

// Here's the syntax for hardware serial (e.g. Arduino Due) --------------
// Un-comment the following line if using hardware serial:

//Adafruit_Thermal printer(&Serial1);      // Or Serial2, Serial3, etc.

// -----------------------------------------------------------------------
char*            PPRINT(char*,char*);  
char*         MM;

void setup(){  




  // This line is for compatibility with the Adafruit IotP project pack,
  // which uses pin 7 as a spare grounding point.  You only need this if
  // wired up the same way (w/3-pin header into pins 5/6/7):
  pinMode(7, OUTPUT); digitalWrite(7, LOW);

  mySerial.begin(19200);  // Initialize SoftwareSerial

  nSerial.begin(9600);
  //Serial1.begin(19200); // Use this instead if using hardware serial
  printer.begin();        // Init printer (same regardless of serial type)

 nSerial.println("AT+CMGF=1"); 
 nSerial.println("AT+CNMI=2,2,0,0,0");
  
 

   // Charset selection alters a few chars in ASCII 0x23-0x7E range.
 //printer.setCharset(CHARSET_NORWAY);
  // Code page selects alt symbols for 'upper' ASCII 0x80-0xFF.
  // There's a TON of these, best to check datasheet!
 //
//
  

  // printer.setCodePage(20);
  // write(uint8_t c);
  // setFont(char font='A');
  dump();


 //printer.println(" دستگاه پرینتر "); 
//printer.printBitmap(adaqrcode_width, adaqrcode_height, adaqrcode_data);
printer.setCodePage(CODEPAGE_IRAN2); 
printer.justify('l');




//printer.println(" دستگاه پرینتر "); 
//printer.println(PPRINT(" میلاد من می "));
MM=(" میلاد من می ");
printer.println(PPRINT(MM));
  printer.feed(2);
  printer.setDefault(); // Restore printer to defaults
}

// Print charset map to printer, similar to test page but
// without the baud rate, etc.
void dump() {
  //uint8_t major, minor, c;

 // printer.println("شطسشیزبلاتئظطزرذد");
        }
                                                   
                                                     


// کلاس پرینت فارسی                                                      



char* PPRINT(char* str){ 
uint8_t i=0, j=0;                                                                                                                    
    while(str[i]){  
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xA2){str[j] = (uint8_t(0x8D)) ; i++;}else //   �
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xA7){str[j] = (uint8_t(0x91)) ; i++;}else //   �

         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xA3){str[j] = (uint8_t(0x90)) ; i++;}else //   �
         
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xA8){str[j] = (uint8_t(0x93)) ; i++;}else// �  
         if(uint8_t(str[i]) == 0xD9 && uint8_t(str[i+1]) == 0xBE){str[j] = (uint8_t(0x95)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xAA){str[j] = (uint8_t(0x97)) ; i++;}else // �
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xAB){str[j] = (uint8_t(0x99)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xAC){str[j] = (uint8_t(0x9B)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xDA && uint8_t(str[i+1]) == 0x86){str[j] = (uint8_t(0x9D)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xAD){str[j] = (uint8_t(0x9F)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xAE){str[j] = (uint8_t(0xA1)) ; i++;}else  //�
         
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xAF){str[j] = (uint8_t(0xA2)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xB0){str[j] = (uint8_t(0xA3)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xB1){str[j] = (uint8_t(0xA4)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xB2){str[j] = (uint8_t(0xA5)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xDA && uint8_t(str[i+1]) == 0x98){str[j] = (uint8_t(0xA6)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD9 && uint8_t(str[i+1]) == 0x88){str[j] = (uint8_t(0xF8)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD9 && uint8_t(str[i+1]) == 0x87){str[j] = (uint8_t(0xFA)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xDB && uint8_t(str[i+1]) == 0x8C){str[j] = (uint8_t(0xFE)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xA1){str[j] = (uint8_t(0x8F)) ; i++;}else //   �
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0x9F){str[j] = (uint8_t(0x8C)) ; i++;}else //   ?
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0x9F){str[j] = (uint8_t(0x8C)) ; i++;}else //   -
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0x9F){str[j] = (uint8_t(0x8C)) ; i++;}else //   .

          if(uint8_t(str[i]) == 0x80 && uint8_t(str[i+1]) == 0x8C){str[j] = (uint8_t(0x20)) ; i++;}else //   .

          if(uint8_t(str[i]) == 0xD9 && uint8_t(str[i+1]) == 0x80){str[j] = (uint8_t(0x8B)) ; i++;}else //   -
         
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xB3){str[j] = (uint8_t(0xA8)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xB4){str[j] = (uint8_t(0xAA)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xB5){str[j] = (uint8_t(0xAC)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xB6){str[j] = (uint8_t(0xAE)) ; i++;}else  //�
         
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xB7){str[j] = (uint8_t(0xAF)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xB8){str[j] = (uint8_t(0xE0)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xB9){str[j] = (uint8_t(0xE3)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xBA){str[j] = (uint8_t(0xE7)) ; i++;}else  //�

         
         if(uint8_t(str[i]) == 0xD9 && uint8_t(str[i+1]) == 0x81){str[j] = (uint8_t(0xEA)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xD9 && uint8_t(str[i+1]) == 0x82){str[j] = (uint8_t(0xEC)) ; i++;}else  //�
         if(uint8_t(str[i]) == 0xDA && uint8_t(str[i+1]) == 0xA9){str[j] = (uint8_t(0xEE)) ; i++;}else  
         if(uint8_t(str[i]) == 0xDA && uint8_t(str[i+1]) == 0xAF){str[j] = (uint8_t(0xF0)) ; i++;}else  
         if(uint8_t(str[i]) == 0xD9 && uint8_t(str[i+1]) == 0x84){str[j] = (uint8_t(0xF3)) ; i++;}else  
         if(uint8_t(str[i]) == 0xD9 && uint8_t(str[i+1]) == 0x85){str[j] = (uint8_t(0xF5)) ; i++;}else  
         if(uint8_t(str[i]) == 0xD9 && uint8_t(str[i+1]) == 0x86){str[j] = (uint8_t(0xF7)) ; i++;}else  
          if(uint8_t(str[i]) == 0xD8 && uint8_t(str[i+1]) == 0xA6){str[j] = (uint8_t(0x8E)) ; i++;}else  //�
                 
      
     {str[j] = (uint8_t) str[i];}  j++; i++;    
    }   while(j<i){str[j]=0; j++;}
 i=0;j=0;



int s=0;

while(str[s]){ 
  s++;
  }
  


char  text[s];

 for (int i = 0; i < s; i++){ 
 text[((s-1)-i)]=uint8_t(str[i]); 
 }

int  o=(strcmp(str,text));



 if (o>0) {
   for (int i = 0; i < s; i++){ 
 text[(i)]=uint8_t(str[i]); 
  }
 
  }else



while(text[i]){ 
  
  
if(uint8_t(text[i]) == 0x91 && uint8_t(text[i+1]) == 0x20) {text[i] = (uint8_t(0x90)) ; }else // �
if(uint8_t(text[i]) == 0x91 && uint8_t(text[i+1]) == 0xA2) {text[i] = (uint8_t(0x90));  }else // �
if(uint8_t(text[i]) == 0x91 && uint8_t(text[i+1]) == 0xA3) {text[i] = (uint8_t(0x90)) ;  }else // �
if(uint8_t(text[i]) == 0x91 && uint8_t(text[i+1]) == 0xA4) {text[i] = (uint8_t(0x90));   }else // �
if(uint8_t(text[i]) == 0x91 && uint8_t(text[i+1]) == 0xA5) {text[i] = (uint8_t(0x90)) ;  }else // �
if(uint8_t(text[i]) == 0x91 && uint8_t(text[i+1]) == 0xA6) {text[i] = (uint8_t(0x90))  ; }else // �
if(uint8_t(text[i]) == 0x91 && uint8_t(text[i+1]) == 0xF8) {text[i] = (uint8_t(0x90)) ;  }else // �
if(uint8_t(text[i]) == 0x91 && uint8_t(text[i-1]) == 0x91) {text[i] = (uint8_t(0x90)) ;  }else // �

if(uint8_t(text[i]) == 0x91 && uint8_t(text[i+1]) == 0x91) {text[i] = (uint8_t(0x90))  ; }else // �


if(uint8_t(text[i]) == 0x93 && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0x92))  ; }else //  �  
if(uint8_t(text[i]) == 0x95 && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0x94))  ; }else //�
if(uint8_t(text[i]) == 0x97 && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0x96)) ;  }else //�
if(uint8_t(text[i]) == 0x99 && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0x98)) ;  }else //�
if(uint8_t(text[i]) == 0x9B && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0x9A)) ;  }else //�
if(uint8_t(text[i]) == 0x9D && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0x9C)) ;  }else //�
if(uint8_t(text[i]) == 0x9F && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0x9E)) ;  }else //�
if(uint8_t(text[i]) == 0xA1 && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xA0)) ;  }else //�
if(uint8_t(text[i]) == 0xA8 && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xA7)) ;  }else //�
if(uint8_t(text[i]) == 0xAA && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xA9)) ;  }else //�
if(uint8_t(text[i]) == 0xAC && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xAB)) ;  }else //�
if(uint8_t(text[i]) == 0xAE && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xAD)) ;  }else //�
if(uint8_t(text[i]) == 0xEA && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xE9)) ;  }else //�
if(uint8_t(text[i]) == 0xEC && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xEB))  ; }else //�
if(uint8_t(text[i]) == 0xEE && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xED))  ; }else //�
if(uint8_t(text[i]) == 0xF0 && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xEF)) ;  }else //�
if(uint8_t(text[i]) == 0xF3 && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xF1)) ;  }else //�



if(uint8_t(text[i]) == 0xF3 && uint8_t(text[i+1]) == 0x91) {text[i] = (uint8_t(0xF3))  ; }else // �

if(uint8_t(text[i]) == 0xF5 && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xF4)) ;  }else //�
if(uint8_t(text[i]) == 0xF7 && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xF6)) ;  }else //�

if(uint8_t(text[i]) == 0xFA && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xF9))   ;}else //�
if(uint8_t(text[i]) == 0xFA && uint8_t(text[i+1]) == 0x20) {text[i] = (uint8_t(0xFB))  ; }else // �

if(uint8_t(text[i]) == 0xFA && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xFB)) ;  }else //�

if(uint8_t(text[i]) == 0xFA && uint8_t(text[i+1]) == 0xA2) {text[i] = (uint8_t(0xF9))  ; }else // �
if(uint8_t(text[i]) == 0xFA && uint8_t(text[i+1]) == 0xA3) {text[i] = (uint8_t(0xF9))  ; }else // �
if(uint8_t(text[i]) == 0xFA && uint8_t(text[i+1]) == 0xA4) {text[i] = (uint8_t(0xF9))  ; }else // �
if(uint8_t(text[i]) == 0xFA && uint8_t(text[i+1]) == 0xA5) {text[i] = (uint8_t(0xF9))  ; }else // �
if(uint8_t(text[i]) == 0xFA && uint8_t(text[i+1]) == 0xA6) {text[i] = (uint8_t(0xF9))  ; }else // �
if(uint8_t(text[i]) == 0xFA && uint8_t(text[i+1]) == 0xF8) {text[i] = (uint8_t(0xF9))  ; }else // �



if(uint8_t(text[i]) == 0xE3 && uint8_t(text[i+1]) == 0x20) {text[i] = (uint8_t(0xE4)) ;  }else //�

if(uint8_t(text[i]) == 0xE3 && uint8_t(text[i+1]) == 0x8D&& uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE1)) ;  }else // �
if(uint8_t(text[i]) == 0xE3 && uint8_t(text[i+1]) == 0x91&& uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE1)) ;  }else // �
if(uint8_t(text[i]) == 0xE3 && uint8_t(text[i+1]) == 0xA2&& uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE1)) ;  }else // �
if(uint8_t(text[i]) == 0xE3 && uint8_t(text[i+1]) == 0xA3&& uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE1));   }else // �
if(uint8_t(text[i]) == 0xE3 && uint8_t(text[i+1]) == 0xA4&& uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE1));   }else // �
if(uint8_t(text[i]) == 0xE3 && uint8_t(text[i+1]) == 0xA5&& uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE1))   ;}else // �
if(uint8_t(text[i]) == 0xE3 && uint8_t(text[i+1]) == 0xA6&& uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE1))  ; }else // �
if(uint8_t(text[i]) == 0xE3 && uint8_t(text[i+1]) == 0xF8&& uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE1)) ;  }else // �
if(uint8_t(text[i]) == 0xE3 && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xE2)) ;  }else //�



if(uint8_t(text[i]) == 0xE7 && uint8_t(text[i+1]) == 0x20) {text[i] = (uint8_t(0xE8));   }else //�

if(uint8_t(text[i]) == 0xE7 && uint8_t(text[i+1]) == 0x91 && uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE5))  ; }else // �
if(uint8_t(text[i]) == 0xE7 && uint8_t(text[i+1]) == 0x8D && uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE5)) ;  }else // �

if(uint8_t(text[i]) == 0xE7 && uint8_t(text[i+1]) == 0xA2 && uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE5));   }else // �
if(uint8_t(text[i]) == 0xE7 && uint8_t(text[i+1]) == 0xA3 && uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE5))  ; }else // �
if(uint8_t(text[i]) == 0xE7 && uint8_t(text[i+1]) == 0xA4 && uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE5)) ;  }else // �
if(uint8_t(text[i]) == 0xE7 && uint8_t(text[i+1]) == 0xA5 && uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE5))   ;}else // �
if(uint8_t(text[i]) == 0xE7 && uint8_t(text[i+1]) == 0xA6 && uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE5))  ; }else // �
if(uint8_t(text[i]) == 0xE7 && uint8_t(text[i+1]) == 0xF8 && uint8_t(text[i-1]) ==0x20) {text[i] = (uint8_t(0xE5)) ;  }else // �
if(uint8_t(text[i]) == 0xE7 && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xE6))  ; }else //�


if(uint8_t(text[i]) == 0xFE && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0xFC))  ; }else //�
if(uint8_t(text[i]) == 0x8E && uint8_t(text[i-1]) == 0x20) {text[i] = (uint8_t(0x8F))  ; }else //�

if(uint8_t(text[i]) == 0x00                              )  {text[i] = (uint8_t(0x00))  ; }else //" "


if(uint8_t(text[i]) == 0x20                              )  {text[i] = (uint8_t(0x20)) ;  }else //" "

if(uint8_t(text[i]) == 0x30                              )  {text[i] = (uint8_t(0x80))  ; }else //0-9
if(uint8_t(text[i]) == 0x31                              )  {text[i] = (uint8_t(0x81))  ; }else //0-9

if(uint8_t(text[i]) == 0x32                              )  {text[i] = (uint8_t(0x82)) ;  }else //0-9
if(uint8_t(text[i]) == 0x33                              )  {text[i] = (uint8_t(0x83))  ; }else //0-9
if(uint8_t(text[i]) == 0x34                              )  {text[i] = (uint8_t(0x84))  ; }else //0-9
if(uint8_t(text[i]) == 0x35                              )  {text[i] = (uint8_t(0x85))  ; }else //0-9
if(uint8_t(text[i]) == 0x36                              )  {text[i] = (uint8_t(0x86))  ; }else //0-9
if(uint8_t(text[i]) == 0x37                              )  {text[i] = (uint8_t(0x87))   ;}else //0-9
if(uint8_t(text[i]) == 0x38                              )  {text[i] = (uint8_t(0x88))   ;}else //0-9
if(uint8_t(text[i]) == 0x39                              )  {text[i] = (uint8_t(0x89))   ;}else //0-9
int b=b+1;
 i++;
  }

for (int i = 0; i < s; i++){ str[i]=(text[i]);  }

return  str;

}
void loop() {
 if (nSerial.available()) {
    String message = nSerial.readString();
    Serial.println("پیامک دریافت شده: " + message);
    //*******
printer.setCodePage(CODEPAGE_IRAN2); 
printer.justify('r');




printer.println(message); 
//printer.println(PPRINT(" میلاد من می "));


//-----


// MM=(" میلاد من می ");
// printer.println(PPRINT(MM));
  printer.feed(2);
  printer.setDefault();
  
//---------


 }
}
