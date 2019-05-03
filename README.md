# Arduino-Lamp
https://kprappcompile.com\n
110-Lab ทดสอบการทำงาน Board Arduino ด้วย LED Build In\n


void setup() {\n
  // initialize digital pin LED_BUILTIN as an output.\n
  pinMode(LED_BUILTIN, OUTPUT);\n
}\n


// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(200);                       // wait for a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(200);                       // wait for a second
}
