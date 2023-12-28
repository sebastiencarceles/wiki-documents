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

## Comment commencer avec Arduino

### Installer l'IDE Arduino

- **Arduino IDE** est un environnement de développement intégré pour Arduino, utilisé pour la programmation logicielle des microcontrôleurs à puce unique, le téléchargement, les tests, etc.
- Téléchargez et installez l'IDE Arduino pour votre système d'exploitation souhaité [ici](https://www.arduino.cc/en/Main/Software).

![](https://files.seeedstudio.com/wiki/Seeeduino_Stalker_V3_1/images/Download_IDE.png)



### Installer le pilote USB

- Arduino se connecte à l'ordinateur via un câble USB. Le pilote USB dépend du type de puce USB que vous utilisez sur votre Arduino. *Remarque : les puces USB sont généralement imprimées à l'arrière de la carte de développement.*

  - Téléchargez le [pilote USB CP2102](https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers). **Remarque : téléchargez en fonction de votre système d'exploitation.**
  - Une fois l'installation du pilote terminée, connectez Arduino au port USB de l'ordinateur à l'aide d'un câble USB.
      - **Pour les utilisateurs de Windows :** Vous pouvez le voir dans `Poste de travail` -> `Propriétés` -> `Matériel` -> `Gestionnaire de périphériques`. Un `COM` apparaîtra.
      - **Pour les utilisateurs de Mac OS :** Vous pouvez accéder à `` dans le coin supérieur gauche, puis choisir `À propos de ce Mac` -> `Rapport système...` -> `USB`. Un pilote USB CP2102 devrait apparaître.
  - Si le pilote n'est pas installé, ou s'il est installé de manière incorrecte (ne correspondant pas au modèle de puce), il apparaîtra comme un "périphérique inconnu" dans le gestionnaire de périphériques. À ce stade, le pilote doit être réinstallé.



### Démarrer l'IDE Arduino

1. Ouvrez l'**IDE Arduino** sur votre ordinateur.
2. Cliquez sur `Outils` -> `Carte` -> `Arduino AVR Boards` -> `Arduino Uno` pour sélectionner le bon modèle de carte de développement. Sélectionnez **Arduino Uno** comme carte.

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/uno_board.jpg)

3. Cliquez sur `Outils` -> `Port` pour sélectionner le bon port (le port série affiché dans le Gestionnaire de périphériques à l'étape précédente). Dans ce cas, `COM11` est sélectionné. **Pour les utilisateurs de Mac OS**, il devrait être `/dev/cu.SLAB_USBtoUART`.

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/port.jpg)


4. Créez un nouveau fichier Arduino et nommez-le `Hello.ino`, puis copiez le code suivant dedans :

```Cpp
void setup() {
  Serial.begin(9600); // initialise le port série avec un débit de 9600 bauds
}
void loop() {
  Serial.println("bonjour, monde"); // imprime une chaîne de caractères sur un port série
  delay(1000); // attend un délai de 1 seconde
}
```

5. Dans le coin supérieur gauche de l'IDE Arduino, il y a deux boutons, **Vérifier et Téléverser**. Appuyez d'abord sur le bouton Vérifier (✓) pour compiler. Après une compilation réussie, appuyez sur le bouton Téléverser (→).

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/func.png)

6. Accédez à `Outils` -> `Moniteur Série`, ou cliquez sur le **Moniteur Série** dans le coin supérieur droit (symbole de la loupe), vous pouvez voir les résultats d'exécution du programme :

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/print.png)

**Remarque :** Si vous avez installé l'IDE Arduino portable à partir de notre clé USB, vous pouvez trouver toutes les démonstrations de modules dans **Fichiers** -> **Carnet de croquis**, ainsi que toutes les bibliothèques de modules, qui sont préinstallées avec l'IDE Arduino !

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/Sketchbook.png)

**Remarque :**
  Tous les modules sont pré-câblés sur une seule carte de circuit imprimé, donc aucun câble ni soudure n'est nécessaire. Cependant, si vous séparez les modules et souhaitez les connecter avec des câbles Grove, veuillez consulter le Guide de séparation.


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
