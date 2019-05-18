<h1>Arduino/NodeMCU ESP8266/Wemos คืออะไร?</h1>

<a href="https://www.wemos.cc/" target="_blank">Link Wemos</a>

<hr>

<h3>Arduino คือ ไมโครคอนโทรลเลอร์ </h3>
<a href="https://www.arduino.cc/" target="_blank">Link Arduino</a>
<a href="https://www.arduino.cc/en/Main/Software" target="_blank">Download Arduino IDE</a>

Arduino เป็นไมโครคอนโทรลเลอร์ที่นำไปใช้อย่างแพร่หลายในปัจจุบัน สามารถเรียนรู้ได้รวดเร็ว จึงเหมาะสำหรับการนำไปสร้างโปรเจ็กต์ ต่างๆ
ไมโครคอนโทรลเลอร์ Arduino ทุกรุ่น จะใช้ชิป AVR เป็นหลัก เพราะมีความทันสมัย 
ไมโครคอนโทรลเลอร์ Arduino สามารถโปรแกรมผ่านพอร์ตอนุกรมชนิต UART ได้ จึงทำให้เขียนโปรแกรมลงไปในชิป โดยการใช้การเชื่อม USB ติดต่อกับ UART

เราสามารถใช้ โปรแกรม Arduino IDE ในการเขียนโปรแกรม และ Upload โปรแกรมลงBoard Arduinoได้ โดยการเชื่อมต่อผ่านสายUSB  เท่านี้เราก็จะได้สนุกกับความาสารของ Board Arduino กันแล้ว 

สามารถ Download โปรแกรม ได้ที่ <a href="https://www.arduino.cc/en/Main/Software" target="_blank">Arduino IDE</a>
    
<h3>ประเภทของ Board Arduino</h3>
<table>
<thead>
<tr>
<th>Type Arduino</th>
<th>Processor</th>
<th>Data Memory</th>
<th>Digital I/O Port</th>
<th>Analog I/O Port</th>
</tr>
</thead>
<tbody>
<tr>
<td>Arduino UNO</td>
<td>16 MHz ATmaga328</td>
<td>2KB SRAM 32 KB Flash</td>
<td>14 Port</td>
<td>6 Port Input</td>
</tr>
<tr>
<td>Arduino Leonardo</td>
<td>16 MHz ATmaga32u4</td>
<td>2.5KB SRAM 32 KB Flash</td>
<td>20 Port</td>
<td>12 Port Input</td>
</tr>
<tr>
<td>Arduino Maga</td>
<td>16 MHz ATmaga2560</td>
<td>8KB SRAM 256 KB Flash</td>
<td>54 Port</td>
<td>16 Port Input</td>
</tr>
<tr>
<td>Arduino Due</td>
<td>84 MHz AT91SAM3X8E</td>
<td>96KB SRAM 512 KB Flash</td>
<td>54 Port</td>
<td>12 Port Input, 2 Port Output</td>
</tr>
</tbody>
</table>
<h3>รูป Boad Arduino</h3>
<table>
<thead>
<th>
<td><h3>1. Arduino UNO</h3></td>
<td><img src="http://www.kprappcompile.com/arduino-img/arduino-uno.png" width="200"></td>
</th>
<th>
<td><h3>2. Arduino Leonardo</h3></td>
<td><img src="http://www.kprappcompile.com/arduino-img/arduino-leonardo.png" width="200"></td>
</th>
<th>
<td><h3>3. Arduino Maga</h3></td>
<td><img src="http://www.kprappcompile.com/arduino-img/arduino-maga.png" width="200"></td>
</th>
<th>
<td><h3>4. Arduino Due</h3></td>
<td><img src="http://www.kprappcompile.com/arduino-img/arduino-due.png" width="200"></td>
</th>
</thead>
</table>


ทั้งนี้ ก็จะมีรุ่นย่อยอื่นอีก เช่น Arduino nano, Arduino Pro mini

อย่างไรก็ดี การเขียน โปรแกรม ก็สามารถเขียนได้เหมือนกัน ทุกรุ่น

<hr>

<h3>Board NodeMCU </h3>

<a href="https://www.espressif.com/en/products/hardware/esp8266ex/overview" target="_blank">Link ESP8266</a>

<a href="https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers">Download Driver CP2102</a>

<a href="https://sparks.gogo.co.nz/ch340.html" target="_blank">Download Driver CH340</a>

   ก่อนที่จะรู้จัก NodeMCU คืออะไรนั้น ก่อนนอื่น เรามารู้จักกับ ESP8266 กันก่อน
ESP8266 เป็นชื่อเรียกของชิฟของโมดูล ESP8266 
ใช้สำหรับติดต่อสื่อสารบนมาตรฐาน WiFi ทำงานที่แรงดันไฟฟ้า 3.0-3.6V นั่นคือเราสารมารเชื่อมต่อ Internet ได้นั่นเอง

เมื่อนำชิฟ ESP8266 มาผลิตเป็นโมดูลหลายรุ่น ก็จะขึ้นต้นด้วย ESP866 แล้วตามด้วยรุ่น เช่น ESP-01 , ESP-03 , ESP-07 , ESP-12

<img src="http://www.kprappcompile.com/arduino-img/esp8266-01.png" width="200">
<img src="http://www.kprappcompile.com/arduino-img/esp8266-03.png" width="200">
<img src="http://www.kprappcompile.com/arduino-img/esp8266-07.png" width="200">
<img src="http://www.kprappcompile.com/arduino-img/esp8266-12.png" width="200">

การใช้งาน การโปรแกรมลงโมดูล ESP8266 มีความไม่สะดวก ต้องต่อผ่าน IC TTL USB เพื่อให้เชื่อมต่อคอมพิวเตอร์ ผ่าน USB Prot ได้
เมื่อโปรแกรมแล้วจึงนำ โมดูล มาใช้งาน

เพื่อให้ง่ายต่อการเขียนโปรแกรม ได้มีการพัฒนาต่อเนื่อง โดยเอา โมดูล ESP8266 ESP-12 มาต่อขยายขา แล้วเพิ่ม IC TTL USB เพิ่มลงในโมดูล
พัฒนา Firmware ให้สามารถเขียนร่วมกับ Arduino IDE ได้ 
จึงกลายมาเป็น NodeMCU ทำให้สามารถเขียนโปรแกรมผ่าน Arduino IDE ได้เหมือน Board Arduino มี Digital Port I/O, Analog Prot 
เช่นเดียวกับ Board Arduino NodeMCU ได้เปลี่ยน Arduino ตรงที่สามารถเชื่อต่อ Internet ได้ 
แต่ก็มีข้อจำกัด NodeMCU มี Digital I/O 11 Port, Analog I/O 1 Port ซึ่งน้อยกว่า Arduino

ปัจจุบัน NodeMCU มีการพัฒนาไปหลายรุ่น 

<h3>Nodemcu V1 (ชื่อที่เป็นทางการ V0.9) ESP8266 ESP-12 ใช้ชิป IC TTL USB CH340 </h3>
    
<img src="http://www.kprappcompile.com/arduino-img/NodeMCU_v0.9_Pinout.png" width="200">
    
 Nodemcu V1 มี Digital I/O 11 Port คือ D0-D10 มี Analog I/O ให้ 1 ช่อง คือ A0

 ทำให้การโปรแกรมมีความสะดวกขึ้นมาก เชื่อมต่อทาง USB ด้วย TTL USB Chip CH340 ความกว้างของ Board 3cm. จึงไม่สามารถวางลงบอร์ดทดลองอันเดียวได้

<h3>Nodemcu V2 (ชื่อที่เป็นทางการ V1.0) ESP8266 ESP-12E TTL USB CP2102</h3>  

<img src="http://www.kprappcompile.com/arduino-img/NodeMCU-V2-Diagram.png" width="200">  

Nodemcu V2 มีคุณสมบัตรใกล้เคียงกับ V1 คือมี Digital I/O 11 Port คือ D0-D10 มี Analog I/O ให้ 1 ช่อง คือ A0

ใช้ชิป ESP8266-12E ใช้ IC TTL USB Chip CP2102 ความกว้างของ Board เล็กกว่า V1 สามารถวางลงบอร์ดทดลองอันเดียวได้ เหลือข้างละ 1 ช่อง


<h3>Nodemcu 3 ESP8266 ESP-12E TTL USB CH340G</h3>
    
<img src="http://www.kprappcompile.com/arduino-img/NodeMCU-V3-Diagram.png" width="200">  

NodeMCU V3 ได้ปรับปรุงจาก NodeMCU V2 โดยเปลี่ยนชิฟ ESP8266-12E เป็น ESP-12F/N ปรับปรุงสายอากาศให้รับส่งสัญญาณได้ดีขึ้น
ทำให้ประสิทธิภาพดีขึ้นมาก เชื่อมต่อทาง USB ด้วย TTL USB Chip CH340 ความกว้างของ Board 3cm. จึงไม่สามารถวางลงบอร์ดทดลองอันเดียวได้
<hr> 
<h3>Board Wemos </h3>
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

