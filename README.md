<h2>Arduino/NodeMCU/Wemos คืออะไร?</h2>
    <p>
        By KPR APP COMPILE มั่นใจด้วยสินค้าคุณภาพ รับประกันทุกชิ้น โปรแกรมผ่าน Arduino IDE
        ผ่าน Board Arduino, Board NodeMCU, Board Wemos
        เรียนรู้ ใช้งาน กับคอร์สเรียน ฟรี พร้อม Source Code และ Driver
    </p>
    
    <h3>Arduino คือ ไมโครคอนโทรลเลอร์ </h3>
    <p>ที่นำไปใช้อย่างแร่หลายในปัจจุบัน สามารถเรียนรู้ได้รวดเร็ว จึงเหมาะสำหรับการนำไปสร้างโปรแจ็กต์ ต่างๆ
        ไมโครคอนโทรลเลอร์ Arduino ทุกรุ่น จะใช้ชิป AVR เป็นหลัก เพราะมีความทันสมัย
        ไมโครคอนโทรลเลอร์ Arduino สามารถโปรแกรมผ่านพอร์ตอนุกรมชนิต UART ได้จึงทำให้เขียนโปรแกรมลงไปในชิป โดยการใช้
        USB ติดต่อกับ UART </p>
    
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

                <td>2.5KB SRAM 32 KB Flash</td>

                <td>20 Port</td>

                <td>12 Port Input</td>
            </tr>

            <tr>

                <td>Arduino Leonardo</td>

                <td>16 MHz ATmaga32u4</td>

                <td>2KB SRAM 32 KB Flash</td>

                <td>14 Port</td>

                <td>6 Port Input</td>
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

                <td>96KB SRAM 512 KB Flash</td>

                <td>54 Port</td>

                <td>12 Port Input, 2 Port Output</td>
            </tr>


        </tbody>
    </table>

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

