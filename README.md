Arduino/NodeMCU/Wemos คืออะไร?

<a href="https://www.arduino.cc/" target="_blank">Arduino</a>

<a href="https://www.espressif.com/en/products/hardware/esp8266ex/overview" target="_blank">ESP8266</a>

<a href="https://www.wemos.cc/" target="_blank">Wemos</a>

Arduino คือ ไมโครคอนโทรลเลอร์ 

Arduino เป็นไมโครคอนโทรลเลิร์ที่นำไปใช้อย่างแพร่หลายในปัจจุบัน สามารถเรียนรู้ได้รวดเร็ว จึงเหมาะสำหรับการนำไปสร้างโปรแจ็กต์ ต่างๆ
ไมโครคอนโทรลเลอร์ Arduino ทุกรุ่น จะใช้ชิป AVR เป็นหลัก เพราะมีความทันสมัย
ไมโครคอนโทรลเลอร์ Arduino สามารถโปรแกรมผ่านพอร์ตอนุกรมชนิต UART ได้จึงทำให้เขียนโปรแกรมลงไปในชิป โดยการใช้USB ติดต่อกับ UART

สามารถใช้ Arduino IDE ในการเขียนโปรแกรม Download ได้ที่ <a href="https://www.arduino.cc/en/Main/Software" target="_blank">Arduino</a>
    
ประเภทของ Board Arduino หลักๆ


1. Arduino UNO

    <img src="http://www.kprappcompile.com/arduino-img/arduino-uno.png" width="200">

    CPU 16 MHz ATmaga328

    2.5KB SRAM 32 KB Flash

    Digital I/O 20 Port

    Analog 12 Port Input

2. Arduino Leonardo

    <img src="http://www.kprappcompile.com/arduino-img/arduino-leonardo.png" width="200">


    CPU 16 MHz ATmaga32u4

    2.5KB SRAM 32 KB Flash

    Digital I/O 20 Port

    Analog 12 Port Input

3. Arduino Maga

    <img src="http://www.kprappcompile.com/arduino-img/arduino-maga.png" width="200">

    CPU 16 MHz ATmaga2560

    8KB SRAM 256 KB Flash

    Digital I/O 54 Port

    Analog 16 Port Input

4. Arduino Due

    <img src="http://www.kprappcompile.com/arduino-img/arduino-due.png" width="200">

    CPU 84 MHz AT91SAM3X8E

    96KB SRAM 512 KB Flash

    Digital 54 Port

    Analog 12 Port Input 2 Port Outpit

ทั้งนี้ ก็จะมีรุ่นย่อยๆอื่นๆอีก เช่น Arduino nano, Arduino Pro mini

อย่างไรก็ดี การเขียน โปรแกรม ก็สามารถเขียนได้เหมือนกัน ทุกรุ่น

NodeMCU 

   ก่อนที่จะรู้จัก NodeMCU คืออะไรนั้น ก่อนนอื่น เรามารู้จักกับ ESP8266 กันก่อน
ESP8266 เป็นชื่อเรียกของชิฟของโมดูล ESP8266 
ใช้สำหรับติดต่อสื่อสารบนมาตรฐาน WiFi ทำงานที่แรงดันไฟฟ้า 3.0-3.6V 

เมื่อนำชิฟ ESP8266 มาผลิตเป็นโมดูลหลายรุ่น ก็จะขึ้นต้นด้วย ESP866 แล้วตามด้วยรุ่น เช่น ESP-01 , ESP-03 , ESP-07 , ESP-12

<img src="http://www.kprappcompile.com/arduino-img/esp8266-01.png" width="200">
<img src="http://www.kprappcompile.com/arduino-img/esp8266-03.png" width="200">
<img src="http://www.kprappcompile.com/arduino-img/esp8266-07.png" width="200">
<img src="http://www.kprappcompile.com/arduino-img/esp8266-12.png" width="200">

เพื่อให้ง่ายต่อการเขียนโปรแกรม ได้มีการพัฒนาต่อเนื่อง โดยเอา โมดูล ESP8266 ESP-12 มาต่อขยายขา แล้วเพิ่ม TTL USB
จึงกลายมาเป็น NodeMCU ที่มีในตลาดปัจจุบัน ก็จะมี 

Nodemcu V1 (ชื่อเรียกอย่างเป็นทางการ V0.9) ESP8266 ESP-12 TTL USB CH340 
    <a href="https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers">Driver CP2102</a> 
   
<img src="http://www.kprappcompile.com/arduino-img/NodeMCU_v0.9_Pinout.png" width="200">
    
Nodemcu V1 มี Digital I/O 11 Port คือ D0-D10 มี Analog I/O ให้ 1 ช่อง คือ A0

ทำให้การโปรแกรมมีความสะดวกขึ้นมาก เชื่อมต่อทาง USB ด้วย TTL USB Chip CH340 

Nodemcu V2 (ชื่อเรียกอย่างเป็นทางการ V1.0) ESP8266 ESP-12E TTL USB CP2102  
    <a href="https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers">Driver CP2102</a>
<img src="http://www.kprappcompile.com/arduino-img/NodeMCU-V2-Diagram.png" width="200">    

Nodemcu 3 ESP8266 ESP-12E TTL USB CH340G
    <a href="https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers">Driver CP2102</a>
<img src="http://www.kprappcompile.com/arduino-img/NodeMCU-V3-Diagram.png" width="200">  

เราจึง นำมาใช่ในงาน IOT กันส่วนใหญ่ เพราะมีความสามารถเขียนโปรแกรมได้เหมือน ที่มีขา Input Output 
        
001-Lab ทดสอบการทำงาน Board Arduino ด้วย LED Build In
เป็น Lab แรกที่จะเรียนรู้เรื่องการทำงานของ Board arduino และ NodeMCU
ใน Code จะมี Function ที่จำเป็นและ ต้องมี 2 Function คือ
1. setup
2. loop

โดยที่ Function setup จะทำงานเริ่มต้น เราจะใช้ Function นี้ ในการ
initialize ค่าเริ่มต้นต่าง

ส่วน Function loop จะทำงานแบบ วนลูป ตลอดการทำงาน

รายละเอียดขาต่างๆ ของ NodeMCU <br>





    void setup() {

        // initialize digital pin LED_BUILTIN as an output.
  
        pinMode(LED_BUILTIN, OUTPUT);
  
    }


    // the loop function runs over and over again forever

    void loop() {

        digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  
        delay(1000);                       // wait for a second => 1000 = 1 second
  
        digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  
        delay(1000);                       // wait for a second => 1000 = 1 second
  
    }
 
 <ul>
    <li><a scr="https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers
 ">Driver TTL CP210x</a></li>
 </ul>

 
 
 
 <img src="https://kprappcompile.app/images/logokpr_webdesign.png" width="150">

