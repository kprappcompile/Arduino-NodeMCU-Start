Arduino/NodeMCU/Wemos คืออะไร?

<a href="https://www.arduino.cc/" target="_blank">Arduino</a>

<a href="https://www.espressif.com/en/products/hardware/esp8266ex/overview" target="_blank">ESP8266</a>

<a href="https://www.wemos.cc/" target="_blank">Wemos</a>

Arduino คือ ไมโครคอนโทรลเลอร์ 

Arduino เป็นไมโครคอนโทรลเลิร์ที่นำไปใช้อย่างแพร่หลายในปัจจุบัน สามารถเรียนรู้ได้รวดเร็ว จึงเหมาะสำหรับการนำไปสร้างโปรแจ็กต์ ต่างๆ
ไมโครคอนโทรลเลอร์ Arduino ทุกรุ่น จะใช้ชิป AVR เป็นหลัก เพราะมีความทันสมัย
ไมโครคอนโทรลเลอร์ Arduino สามารถโปรแกรมผ่านพอร์ตอนุกรมชนิต UART ได้จึงทำให้เขียนโปรแกรมลงไปในชิป โดยการใช้USB ติดต่อกับ UART
    
<u>ประเภทของ Board Arduino หลักๆ</u>


1. Arduino UNO

    <img src="http://www.kprappcompile.com/arduino-img/arduino-uno.png" width="200">

    CPU 16 MHz ATmaga328

    2.5KB SRAM 32 KB Flash

    Digital 20 Port

    Analog 12 Port Input

2. Arduino Leonardo

    <img src="http://www.kprappcompile.com/arduino-img/arduino-leonardo.png" width="200">


    CPU 16 MHz ATmaga32u4

    2.5KB SRAM 32 KB Flash

    Digital 20 Port

    Analog 12 Port Input

3. Arduino Maga

    <img src="http://www.kprappcompile.com/arduino-img/arduino-maga.png" width="200">

    CPU 16 MHz ATmaga2560

    8KB SRAM 256 KB Flash

    Digital 54 Port

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

ESP8266 มีรุ่นย่อยๆหลายรุ่น โดยหลักๆแล้วทำงานเหมือนกัน

<img src="http://www.kprappcompile.com/arduino-img/esp8266-01.png" width="200">
<img src="http://www.kprappcompile.com/arduino-img/esp8266-03.png" width="200">
<img src="http://www.kprappcompile.com/arduino-img/esp8266-07.png" width="200">
<img src="http://www.kprappcompile.com/arduino-img/esp8266-12.png" width="200">




ใช้สำหรับติดต่อสื่อสารบนมาตรฐาน WiFi ทำงานที่แรงดันไฟฟ้า 3.0-3.6V 

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

