stepper
=======
void setup() {
  // put your setup code here, to run once:
pinMode(8,OUTPUT);
pinMode(9,OUTPUT);
pinMode(10,OUTPUT);
pinMode(11,OUTPUT);
Serial.begin(9600);
}

void loop() {
byte time; // put your main code here, to run repeatedly:
if(Serial.available()){
  time = Serial.read();
digitalWrite(8,HIGH);
delay(time);
digitalWrite(8,LOW);
delay(time);
digitalWrite(9,HIGH);
delay(time);
digitalWrite(9,LOW);
delay(time);
digitalWrite(10,HIGH);
delay(time);
digitalWrite(10,LOW);
delay(time);
digitalWrite(11,HIGH);
delay(time);
digitalWrite(11,LOW);
delay(time);
}
}


Stepper  
