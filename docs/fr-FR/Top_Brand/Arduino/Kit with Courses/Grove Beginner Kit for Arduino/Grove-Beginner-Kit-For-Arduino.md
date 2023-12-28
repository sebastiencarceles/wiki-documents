---
description: Kit débutant Grove pour Arduino
title: Kit débutant Grove pour Arduino
keywords:
- Kit avec cours
image: https://files.seeedstudio.com/wiki/wiki-platform/S-tempor.png
slug: /Grove-Beginner-Kit-For-Arduino-fr-FR
last_update:
  date: 12/27/2023
  author: sebastiencarceles
---
# Grove Beginner Kit For Arduino

Le kit débutant Grove pour Arduino est l'un des meilleurs kits Arduino pour les débutants. Il comprend une carte compatible Arduino et 10 capteurs Arduino supplémentaires, le tout dans un seul design de carte PCB. **Tous les modules ont été connectés au Seeeduino via les trous de la carte PCB, donc aucun câble Grove n'est nécessaire pour les connecter**. Bien sûr, vous pouvez également retirer les modules et utiliser des câbles Grove pour les connecter. Vous pouvez construire n'importe quel projet Arduino que vous souhaitez avec ce kit débutant Grove pour Arduino.

<div class="get_one_now_container" style={{textAlign: 'center'}}>
    <a class="get_one_now_item" href="https://www.seeedstudio.com/Grove-Beginner-Kit-for-Arduino-p-4549.html">
            <strong><span><font color={'FFFFFF'} size={"4"}> Obtenez le vôtre maintenant 🖱️</font></span></strong>
    </a>
</div>

## Hardware Overview

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/Parts.jpg)

**Note:** Dimensions - 17.69 * 11.64 * 1.88cm

1. **[Grove - LED](https://wiki.seeedstudio.com/Grove-Red_LED/):** Module LED simple
2. **[Grove - Buzzer](https://wiki.seeedstudio.com/Grove-Buzzer/):** Buzzer piézoélectrique
3. **[Grove - OLED Display 0.96"](https://wiki.seeedstudio.com/Grove-OLED-Display-0.96-SSD1315/):** Écran compact à faible consommation d'énergie. Résolution de 128×64 points, luminosité élevée, auto-émission et rapport de contraste élevé
4. **[Grove - Button](https://wiki.seeedstudio.com/Grove-Button/):** Bouton poussoir
5. **[Grove - Rotary Potentiometer](https://wiki.seeedstudio.com/Grove-Rotary_Angle_Sensor/):** Potentiomètre réglable
6. **[Grove - Light](https://wiki.seeedstudio.com/Grove-Light_Sensor/):** Détecte l'intensité lumineuse environnante
7. **[Grove - Sound](https://wiki.seeedstudio.com/Grove-Sound_Sensor/):** Détecte l'intensité sonore environnante
8. **[Grove - Temperature & Humidity Sensor](https://wiki.seeedstudio.com/Grove-TemperatureAndHumidity_Sensor/):** Détecte les valeurs de température et d'humidité environnantes
9. **[Grove - Air Pressure Sensor](https://wiki.seeedstudio.com/Grove-Barometer_Sensor-BMP280/):** Détecte la pression atmosphérique environnante
10. **[Grove - 3-Axis Accelerator](https://wiki.seeedstudio.com/Grove-3-Axis-Digital-Accelerometer-LIS3DHTR):** Détecte l'accélération
11. **[Seeeduino Lotus](https://wiki.seeedstudio.com/Seeeduino_Lotus/):** Carte compatible Arduino avec ports Grove


**Note:**
        Par défaut, les modules Grove sont connectés à Seeeduino via les trous de la carte PCB. Cela signifie que vous n'avez pas besoin d'utiliser des câbles Grove pour les connecter si ils ne sont pas séparés. Les broches par défaut sont les suivantes :

|Modules|Interface|Pins/Address|
|---|---|---|
|LED|Digital|D4|
|Buzzer|Digital|D5|
|OLED Display 0.96"|I2C|I2C, 0x78(default)|
|Button|Digital|D6|
|Rotary Potentiometer|Analog|A0|
|Light|Analog|A6|
|Sound|Analog|A2|
|Temperature & Humidity Sensor|Digital|D3|
|Air Pressure Sensor|I2C|I2C, 0x77(default) / 0x76(optional)|
|3-Axis Accelerator|I2C|I2C, 0x19(default)|
 


### Instructions pour séparer les modules

**Attention :**
  Veuillez faire attention à ne pas vous couper lorsque vous utilisez un couteau.


Si vous préférez utiliser les modules ailleurs que sur la carte Seeeduino, vous pouvez simplement suivre les instructions suivantes pour séparer les modules !

**Étape 1**

Utilisez un couteau ou un objet tranchant pour couper au niveau des trous de découpe qui relient les capteurs entre eux.

**Étape 2**

Secouez les modules de haut en bas et ils devraient se séparer assez facilement !


## Liste des pièces

|Modules|Quantité|
|---|---|
|---|---|
|**Sensors**||
|Temperature & Humidity Sensors|x1|
|3-Axis Accelerometers|x1|
|Air Pressure|x1|
|Light Sensor|x1|
|Sound Sensor|x1|
|**Input Modules**||
|Rotary Potentiometer|x1|
|Button|x1|
|**Output Modules**||
|LED|x1|
|Buzzer|x1|
|**Display Module**||
|OLED Display|x1|
|**Grove Cables**|x6|
|**Micro USB Cable**|x1|


## Objectifs d'apprentissage

- Bases des systèmes de matériel open source.
- Programmation Arduino de base.
- Principes de communication et méthodes pour les capteurs.
- Mise en œuvre pratique de projets de matériel open source.

### Démonstration Plug and Play

Le kit débutant Grove dispose d'une démonstration plug and play, où vous branchez d'abord l'alimentation sur la carte, et vous avez la chance de découvrir tous les capteurs en une seule fois ! Utilisez le bouton et le potentiomètre rotatif pour découvrir chaque démonstration de capteur !

![](https://s3-us-west-2.amazonaws.com/files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/Firmware.jpg)

- **Défilement** -> Rotation du potentiomètre rotatif
- **Sélection** -> Appui court sur le bouton
- **Quitter la démo en cours** -> Appui long sur le bouton

Le module Buzzer et LED sont utilisés pour donner des indications.

## How to Get Started With Arduino

### Install the Arduino IDE

- **Arduino IDE** is an integrated development environment for Arduino, which is used for single-chip microcomputer software programming, downloading, testing and so on.
- Download and Install [Arduino IDE](https://www.arduino.cc/en/Main/Software) for your desired operating system here.

![](https://files.seeedstudio.com/wiki/Seeeduino_Stalker_V3_1/images/Download_IDE.png)



### Install the USB driver

- Arduino connects to the PC via a USB cable. The USB driver depends on the type of USB chip you're using on your Arduino. *Note: USB chips are usually printed on the back of the development board.*

  - Download the [CP2102 USB Driver](https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers). **Note:** Download according to your OS.
  - After the driver installation is completed, connect Arduino to the USB port of PC with a USB cable. 
      - **For Windows users:** You can see it in `My Computer` -> `Properties` -> `Hardware` -> `Device Management`. A `COM` will appear.
      - **For Mac OS users:** You can navigate to `` on the top left corner, and choose `About this Mac` -> `System Report...` -> `USB`. A CP2102 USB Driver should appear.
  - If the driver is not installed, or if the driver is installed incorrectly (not matching the chip model), it will appear as an "unknown device" in the device manager. At this point, the driver should be reinstalled.



### Start the Arduino IDE

1.Open the **Arduino IDE** on your PC.
2.Click on `Tools` -> `Board`-> `Arduino AVR Boards`-> `Arduino Uno` to select the correct Development Board Model. Select **Arduino Uno** as Board.

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/uno_board.jpg)

3.Click `Tools` -> `Port` to select the correct Port (the Serial Port showed in Device Manager in the previous step). In this case, `COM11` is selected. **For Mac OS users**, it should be `/dev/cu.SLAB_USBtoUART`.

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/port.jpg)


4.Create a new Arduino file and name it `Hello.ino`, then copy the following code into it:

```Cpp
void setup() {
  Serial.begin(9600); // initializes the serial port with a baud rate of 9600
}
void loop() {
  Serial.println("hello, world"); // prints a string to a serial port
  delay(1000); //delay of 1 second
}
```

5.In the upper left corner of the Arduino IDE, there are two buttons, **Verify and Upload**. First, press the Verify button(✓) to compile. After the compilation is successful, press the upload button(→).

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/func.png)

6.Navigate to `Tools` -> `Serial Monitor`, or click the **Serial Monitor** in the upper right corner(Magnifier Symbol), you can see the program running results:

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/print.png)

**Note:** If you installed the portable Arduino IDE from our USB Drive, you can find all the module demos in the **Files** -> **Sketch Book**, as well as all the module libraries, are pre-installed with Arduino IDE!

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/Sketchbook.png)

**Note:**
        All modules are pre-wired on a single circuit board, so no cables and soldering are needed. However, if you break out the modules and want to connect them with Grove  cables, please kindly check the Breakout Guide.


## Lesson Guide

### Lesson 1: Blinking with the LED

We have completed the output "Hello world" program. Now let's learn how to light the LED module. We know the three basic components of a control system: Input, Control, and Output. But lighting up LED uses only the output, not the input. Seeeduino is the control unit, the LED module is the output unit and the output signal is a digital signal.

Background Information:


- **What is Digital Signal**

**Digital signal:** Digital signal refers to the value of the amplitude is discrete, the amplitude is limited to a finite number of values. In our controller, the digital signal has two states: LOW(0V) for 0; HIGH(5V) for 1. So sending a HIGH signal to LED can light it up.

![Alt text](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/digital.png)



Components Involved
    1. Seeeduino Lotus
    2. Grove LED
    3. Grove Cable(If Broken out)

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/LED.png)


Hardware connection
    - **Module connection**
        - Default connection by PCB stamp hole.
    - Connect the Seeeduino to the computer through the USB cable.


-Software Code

    - Open Arduino IDE.
    - Copy the following code, click Verify to check for syntax errors. Verify that there are no errors, and you can upload the code.

```Cpp
//LED Blink
//The LED will turn on for one second and then turn off for one second
int ledPin = 4;
void setup() {
    pinMode(ledPin, OUTPUT);
}
void loop() {
    digitalWrite(ledPin, HIGH);
    delay(1000);
    digitalWrite(ledPin, LOW);
    delay(1000);
}
```





Code Analysis


```cpp
setup(){
}
```

The `setup()` function is called when a sketch starts. Use it to initialize variables, pin modes, start using libraries, etc. The `setup()` function will only run once, after each powerup or reset of the Arduino board.

```cpp
loop(){
}
```

After creating a `setup()` function, which initializes and sets the initial values, the `loop()` function does precisely what its name suggests, and loops consecutively, allowing your program to change and respond. Use it to actively control the Arduino board.

```cpp
int ledPin = 4;
```

**Description:**

Converts a value to the int data type.

**Syntax:**

int(**x**) or (int)**x** (C-style type conversion)

**Parameters:**

**x**: a value. Allowed data types: any type.

Assigned an `int` type 4 to variable named ledPin.

```cpp
pinMode(ledPin, OUTPUT);
```

**Description:**

Configures the specified pin to behave either as an input or an output. See the Digital Pins page for details on the functionality of the pins.

As of Arduino 1.0.1, it is possible to enable the internal pull-up resistors with the mode `INPUT_PULLUP`. Additionally, the `INPUT` mode explicitly disables the internal pullups.

**Syntax:**

pinMode(**pin, mode**)

**Parameters:**

**pin**: the Arduino pin number to set the mode of.

**mode**: `INPUT`, `OUTPUT`, or `INPUT_PULLUP`.

Setting ledPin to the output mode.

```cpp
digitalWrite(ledPin, HIGH);
```

**Description:**

Write a `HIGH` or a `LOW` value to a digital pin.

If the pin has been configured as an OUTPUT with pinMode(), its voltage will be set to the corresponding value: 5V (or 3.3V on 3.3V boards) for `HIGH`, 0V (ground) for `LOW`.

If the pin is configured as an INPUT, digitalWrite() will enable (HIGH) or disable (LOW) the internal pullup on the input pin. It is recommended to set the pinMode() to `INPUT_PULLUP` to enable the internal pull-up resistor. See the Digital Pins tutorial for more information.

If you do not set the pinMode() to OUTPUT, and connect an LED to a pin, when calling digitalWrite(HIGH), the LED may appear dim. Without explicitly setting pinMode(), digitalWrite() will have enabled the internal pull-up resistor, which acts as a large current-limiting resistor.

**Syntax:**

digitalWrite(**pin, value**)

**Parameters:**

**pin**: the Arduino pin number.

**value**: `HIGH` or `LOW`.

When we set the ledPin as output, HIGH means sending high level to the pin, LED turns on.

```cpp
digitalWrite(ledPin, LOW);
```

When we set the led as output, low stands for sending low level to the pin, LED turns off.

```cpp
delay(1000);
```

**Description:**

Pauses the program for the amount of time (in milliseconds) specified as a parameter. (There are 1000 milliseconds in a second.)

**Syntax:**

delay(**ms**)

**Parameters:** 

**ms**: the number of milliseconds to pause. Allowed data types: unsigned long.

Delay the program by 1000ms(1s).

**Demo Effect and Serial Print Result:**

The LED module will be 1 second on and 1 second off.

**LED Brightness Adjustment:**

<div>
  <div align="center"><img src="https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/LED-res.jpeg" /></div>
  <br />
</div>


On the Grove LED module, there is a **variable resistor that can be adjusted using a screw driver.** Twist it to make the LED light up brighter!


Breakout Guide


If modules are broken out from the board. Use a Grove cable to connect the **Grove LED** to Seeeduino Lotus's digital interface **D4**.  





### Lesson 2: Pressing Button to Light Up LED
