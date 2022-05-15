## Introduction

This site is to document the projects and experiments done as a part of kerala iot challenge.Kerala IoT Challenge is a program designed in 4 levels followed by a hackathon to identify and train quality industry leaders in the IoT domain, while any novice learner can start with layer 1 and others can enter laterally to the desired layer after an evaluation.

## About me

Iam SALMAN FARIS Btech Computer Science And Engineering Student At Cochin University Of Science And Technology, Ernakulam, Kerala, India. I love to learn tehnology and try new things. I also love to code and play video games. Iam passionate about computer science. Iam a web developer currently working as a freelancer and part time developer. Iam always ready to work on cool projects and contribute to open source. Feel free to contact me for collaboration or any kind of stuffs related to computer science. connect with me through Linkedin

## Level 1

This section contains the experiments and projects done as a part of kerala iot challenge level 1

**Level 1 consists of basic electronics, sensors, arduino programming and a live project


# Experiments
This section contains the experiments done as part of kerala iot challenge level 1



## Experiment 1 : Hello World Led Blinking

<u>Components Required</u>

- Arduino Uno Board
- USB Cable
- LED (Any Color) x 1 Nos
- 220 OHM Resistor X 1 Nos
- Breadboard
- Jumper Wires (Male to Male ) X 2 Nos

Circuit diagram

![image](https://user-images.githubusercontent.com/76479492/168489390-af2e073a-d1cd-46a4-8d67-4f8c249b6bc5.png)


<u>Code</u>
```C++
int ledPin = 10; // define digital pin 10.
void setup()
{
pinMode(ledPin, OUTPUT);// define pin with LED connected as output.
}
void loop()
{
digitalWrite(ledPin, HIGH); // set the LED on.
delay(1000); // wait for a second.
digitalWrite(ledPin, LOW); // set the LED off.
delay(1000); // wait for a second
}
```

Result: https://youtube.com/shorts/R-UdT4j3jIo?feature=share



## Experiment 2 : Traffic Light

<U>Components Required</U>

- Arduino board *1
- USB cable *1
- Red M5 LED*1
- Yellow M5 LED*1
- Green M5 LED*1
- 220Ω resistor *3
- Breadboard*1
- Breadboard jumper wires* several

Circuit Diagram
![image](https://user-images.githubusercontent.com/76479492/168489833-cbcf01e5-0e17-43f0-b969-17f579e41921.png)

<U>Code</U>

```C++
int redled =10; // initialize digital pin 8.
int yellowled =7; // initialize digital pin 7.
int greenled =4; // initialize digital pin 4.
void setup()
{
pinMode(redled, OUTPUT);// set the pin with red LED as “output”
pinMode(yellowled, OUTPUT); // set the pin with yellow LED as “output”
pinMode(greenled, OUTPUT); // set the pin with green LED as “output”
}
void loop()
{
digitalWrite(greenled, HIGH);//// turn on green LED
delay(5000);// wait 5 seconds

digitalWrite(greenled, LOW); // turn off green LED
for(int i=0;i<3;i++)// blinks for 3 times
{
delay(500);// wait 0.5 second
digitalWrite(yellowled, HIGH);// turn on yellow LED
delay(500);// wait 0.5 second
digitalWrite(yellowled, LOW);// turn off yellow LED
} 
delay(500);// wait 0.5 second
digitalWrite(redled, HIGH);// turn on red LED
delay(5000);// wait 5 seconds
digitalWrite(redled, LOW);// turn off red LED
}
```

Result:
https://youtube.com/shorts/1qBPqKji2PU?feature=share


### Experiment 3 : Led Chasing effect

**Components Required

- Led *6
- Arduino board *1
- 220Ω resistor *6
- Breadboard *1
- USB cable*1
- Breadboard wire *13

Circuit diagram
![image](https://user-images.githubusercontent.com/76479492/168490096-31e4a106-7dcd-4714-ac66-15b856b37843.png)

<U>Code</u>
```C++
int BASE = 2 ;  // the I/O pin for the first LED
int NUM = 6;   // number of LEDs
void setup()
{
   for (int i = BASE; i < BASE + NUM; i ++) 
   {
     pinMode(i, OUTPUT);   // set I/O pins as output
   }
}
void loop()
{
   for (int i = BASE; i < BASE + NUM; i ++) 
   {
     digitalWrite(i, LOW);    // set I/O pins as “low”, turn off LEDs one by one.
     delay(200);        // delay
   }
   for (int i = BASE; i < BASE + NUM; i ++) 
   {
     digitalWrite(i, HIGH);    // set I/O pins as “high”, turn on LEDs one by one
     delay(200);        // delay
   }  
}
```
Result:
https://youtube.com/shorts/_Pdv6C-6l-0?feature=share



### Experiment 4 : Button Controlled Led

***Components Required

- Arduino Uno
- Button switch*1
- Red M5 LED*1
- 220ΩResistor*1
- 10KΩ Resistor*1
- Breadboard*1
- Breadboard Jumper Wire*6
- USB cable*1

Circuit Diagram
![image](https://user-images.githubusercontent.com/76479492/168490407-7126e72a-9b76-43f8-8f02-825531227080.png)


<U>Code</U>
```C++
int ledpin=11;// initialize pin 11
int inpin=7;// initialize pin 7
int val;// define val
void setup()
{
pinMode(ledpin,OUTPUT);// set LED pin as “output”
pinMode(inpin,INPUT);// set button pin as “input”
}
void loop()
{
val=digitalRead(inpin);// read the level value of pin 7 and assign if to val
if(val==LOW)// check if the button is pressed, if yes, turn on the LED
{ digitalWrite(ledpin,LOW);}
else
{ digitalWrite(ledpin,HIGH);}
}
```

Result:
https://youtube.com/shorts/57EHzPsuxh4?feature=share


### Experiment 5 : Buzzer

**Components Required

- Arduino Uno
- Buzzer*1
- Breadboard*1
- Breadboard Jumper Wire*2
- USB cable*1

Circuit Diagram
![image](https://user-images.githubusercontent.com/76479492/168490980-2dca127d-d4aa-4af0-aab3-be71800dbb0f.png)


<U>Code</U>
```C++
int buzzer=8;// initialize digital IO pin that controls the buzzer
void setup() 
{ 
  pinMode(buzzer,OUTPUT);// set pin mode as “output”
} 
void loop() 
{
digitalWrite(buzzer, HIGH); // produce sound
}
}
```

Result:
https://youtube.com/shorts/uRBJG3MW1yE?feature=share


### Experiment 6 : RGB Led

**Components Required

- Arduino Uno
- USB Cable * 1
- RGB LED * 1
- Resistor *3
- Breadboard jumper wire*5

Circuit Diagram
![image](https://user-images.githubusercontent.com/76479492/168491181-65f56d39-cde7-433f-8081-735bfda106d1.png)

<u>Code</u>
```c++
int redpin = 11; //select the pin for the red LED
int bluepin =10; // select the pin for the blue LED
int greenpin =9;// select the pin for the green LED
int val;
void setup() {
  pinMode(redpin, OUTPUT);
  pinMode(bluepin, OUTPUT);
  pinMode(greenpin, OUTPUT);
  Serial.begin(9600);
}
void loop() 
{
for(val=255; val>0; val--)
  {
   analogWrite(11, val);
   analogWrite(10, 255-val);
   analogWrite(9, 128-val);
   delay(1); 
  }
for(val=0; val<255; val++)
  {
   analogWrite(11, val);
   analogWrite(10, 255-val);
   analogWrite(9, 128-val);
   delay(1); 
  }
 Serial.println(val, DEC);
}
```

Result:
https://youtube.com/shorts/6rslwnvuu0M?feature=share


### Experiment 7 : LDR Light Sensor

**Components Required

- Arduino Uno Board
- Photo Resistor*1 or LDR Module(Iam using LDR Module)
- Red M5 LED*1
- 10KΩ Resistor*1
- 220Ω Resistor*1
- Breadboard*1
- Breadboard Jumper Wire*5
- USB cable*1
