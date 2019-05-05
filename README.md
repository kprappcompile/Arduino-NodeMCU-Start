# Arduino NodeMCU 

https://kprappcompile.com

001-Lab ทดสอบการทำงาน Board Arduino ด้วย LED Build In
เป็น Lab แรกที่จะเรียนรู้เรื่องการทำงานของ Board arduino และ NodeMCU
ใน Code จะมี Function ที่จำเป็นและ ต้องมี 2 Function คือ
1. setup
2. loop

โดยที่ Function setup จะทำงานเริ่มต้น เราจะใช้ Function นี้ ในการ
initialize ค่าเริ่มต้นต่าง

ส่วน Function loop จะทำงานแบบ วนลูป ตลอดการทำงาน

รายละเอียดขาต่างๆ ของ NodeMCU <br>
<div style="align-center">
<img src="https://www.arduinoall.net/arduino-tutor/wp-content/uploads/2016/11/NodeMCU__v1.0_pinout1.jpg" width="700">
</div>




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
 <img src="https://kprappcompile.app/images/logokpr_webdesign.png" width="150">

