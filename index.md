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


Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Salmanfaris687/keralaIOTchallenge/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
