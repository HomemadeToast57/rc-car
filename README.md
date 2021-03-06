# LEGO RC Car
A classic toy for kids now modernized and controllable from any bluetooth device.

![car](https://user-images.githubusercontent.com/54961512/135902374-ed2175e5-dd5b-4d50-93cf-df328c00e580.jpg)

### How It Began
##### Research
We decided to retrofit a childhood toy with bluetooth, RGB lights, a gearbox motor, and a servo to make it actually functional.

### Why
##### Empathize/Define
Like us, due to Covid-19, many people are stuck at home looking for things to keep them occupied. Building cars like ours provides a fun, easy, and educational way to spend your time. It builds problem solving skills while enhancing your knowledge of circuitry, C++, and Arduino. All that is required to do this on your own is a lego set large enough to accommodate all of the components (I used the LEGO Technic Extreme Cruiser), an Arduino, a bluetooth module, a servo motor, a gearbox motor, wires, and a bluetooth compatible device. You can even add LEDs, a piezo buzzer, and much more like we did.

### Problem Solving
##### Ideate/Prototype
While building this car we faced many challenges. For example, it was difficult to collaborate on it as only one person has the physical device. Also, without a lab full of supplies it was hard to obtain the components required. Another major challenge we faced was powering the vehicle. We began powering the car with two 9 volt and four AA batteries. However, this wasn't enough power. When the car turned, it would reset the Arduino and disconnect the bluetooth. After doing some research and brainstorming we decided to switch out a 9 volt battery and the AAs for a 12 volt lithium ion battery. This change improved the cars battery however it did not fix the problem. After large turns, the Arduino would still reset and the bluetooth would disconnect. To fix this problem we added a delay in the servo code to make it turn slightly slower causing less battery consumption and fixing the problem. Some other challenges we faced were connecting the motor to the drive shaft, correcting the tie rods allignment to prevent uneven turning, fitting the battery and other components in the car, and much more.

### Methods
#### Servo
Begin by connecting the servo to pin 9 on the Arduino and connecting that to the mechanism that turns the wheels.

#### Motor/Transistor
Next, connect the motor to the drive shaft with its power connected to the VCC pin and the ground connected to the middle pin of the transistor. Connect a battery (we used a 9 volt) to the 5 volt pin. Connect the ground of the battery and the ground of the transistor (the pin to the right) to the ground of the Arduino. Connect the final pin of the transistor (the pin to the left) to pin 8.

#### Bluetooth Module
Connect the TX, RX, GND, and VCC pins on the bluetooth module to pins 10, 11, ground, and 5 volts respectively on the Arduino.

#### Lights
Connect the lights' power to pin 13 on the Arduino and their ground to ground.

#### Horn(buzzer)
Connect the power for the buzzer to pin 12 on the Arduino and its ground to ground.

#### Code/Power
Finally, connect a large battery to the AC power port (we used a 12 volt lithium ion) and plug the Arduino into a computer. Now, just upload the code below, and you are finished!

### Credit

<b>Engineered By [Isaac Zipperstein](https://github.com/AplAddict) and Programmed By [Jacob Singer](https://github.com/HomemadeToast57).</b>
