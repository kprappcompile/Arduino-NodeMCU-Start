Arduino/NodeMCU/Wemos คืออะไร?

By KPR APP COMPILE มั่นใจด้วยสินค้าคุณภาพ รับประกันทุกชิ้น โปรแกรมผ่าน Arduino IDE
ผ่าน Board Arduino, Board NodeMCU, Board Wemos
เรียนรู้ ใช้งาน กับคอร์สเรียน ฟรี พร้อม Source Code และ Drive
    
Arduino คือ ไมโครคอนโทรลเลอร์ 

ที่นำไปใช้อย่างแร่หลายในปัจจุบัน สามารถเรียนรู้ได้รวดเร็ว จึงเหมาะสำหรับการนำไปสร้างโปรแจ็กต์ ต่างๆ
ไมโครคอนโทรลเลอร์ Arduino ทุกรุ่น จะใช้ชิป AVR เป็นหลัก เพราะมีความทันสมัย
ไมโครคอนโทรลเลอร์ Arduino สามารถโปรแกรมผ่านพอร์ตอนุกรมชนิต UART ได้จึงทำให้เขียนโปรแกรมลงไปในชิป โดยการใช้USB ติดต่อกับ UART </p>
    
ประเภทของ Board Arduino

1. Arduino UNO

    <img sec="http://www.kprappcompile.com/arduino-img/arduino-uno.png" width="200">

    CPU 16 MHz ATmaga328

    2.5KB SRAM 32 KB Flash

    Digital 20 Port

    Analog 12 Port Input

2. Arduino Leonardo

    CPU 16 MHz ATmaga32u4

    2.5KB SRAM 32 KB Flash

    Digital 20 Port

    Analog 12 Port Input

3. Arduino Maga

    CPU 16 MHz ATmaga2560

    8KB SRAM 256 KB Flash

    Digital 54 Port

    Analog 16 Port Input

4. Arduino Due

    CPU 84 MHz AT91SAM3X8E

    96KB SRAM 512 KB Flash

    Digital 54 Port

    Analog 12 Port Input 2 Port Outpit
        
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

