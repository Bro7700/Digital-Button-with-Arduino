# Digital-Button-with-Arduino
Task 5



## Introduction


 control LEDs with code, which is one use for Arduino's outputs. This circuit builds on outputs by adding an input. Your Arduino board can be programmed to listen to electrical signals and take actions based on those inputs. A pushbutton is one kind of switch a mechanical device that connects or breaks a circuit.






## Technologies


1- Arduino IDE 1.8.19 [To Download](https://www.arduino.cc/en/software)



2- AUTODESK TINKERCAD [To Download](https://www.tinkercad.com/)






## Components required



1. Arduino UNO
2. Push Button
3. jumper wirs
4. LED Light
5. Resistor




## Connections


connecting push button to Pin 2  and connecting GNR with Resistor and 5V in Arduino

connecting LED Light to Pin 13 with resistor and connecting LED to GNR in Arduino








## Block diagram & simulation


for watching simulation [OPEN](https://www.tinkercad.com/things/9NfdFfCHIqB-spectacular-wluff/editel?tenant=circuits)



![Spectacular Wluff (1)](https://user-images.githubusercontent.com/109243989/182015169-0a5a65e2-40ae-4e75-8234-a958a54d125a.png)







#### The Code



int buttonState = 0;

void setup()
{
  pinMode(2, INPUT);
  pinMode(13, OUTPUT);
}

void loop()
{
  // read the state of the pushbutton
  buttonState = digitalRead(2);
  // check if pushbutton is pressed. if it is, the
  // button state is HIGH
  if (buttonState == HIGH) {
    digitalWrite(13, HIGH);
  } else {
    digitalWrite(13, LOW);
  }
  delay(10); // Delay a little bit to improve simulation performance
}


