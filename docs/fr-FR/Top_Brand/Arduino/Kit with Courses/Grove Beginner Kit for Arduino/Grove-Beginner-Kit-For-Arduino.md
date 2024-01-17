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


## Guide de leçon

### Leçon 1 : Clignotement avec la LED

Nous avons terminé le programme de sortie "Hello world". Maintenant, apprenons comment allumer le module LED. Nous connaissons les trois composants de base d'un système de contrôle : Entrée, Contrôle et Sortie. Mais l'allumage de la LED utilise uniquement la sortie, pas l'entrée. Seeeduino est l'unité de contrôle, le module LED est l'unité de sortie et le signal de sortie est un signal numérique.

Informations de base :

- **Qu'est-ce qu'un signal numérique**

**Signal numérique :** Un signal numérique fait référence à une valeur d'amplitude discrète, l'amplitude étant limitée à un nombre fini de valeurs. Dans notre contrôleur, le signal numérique a deux états : LOW (0V) pour 0 ; HIGH (5V) pour 1. Ainsi, l'envoi d'un signal HIGH à la LED peut l'allumer.

![Alt text](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/digital.png)

Composants impliqués :
  1. Seeeduino Lotus
  2. Grove LED
  3. Câble Grove (si nécessaire)

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/LED.png)

Connexion matérielle :
  - **Connexion du module**
    - Connexion par défaut via le trou de la carte PCB.
  - Connectez le Seeeduino à l'ordinateur via le câble USB.

- Code logiciel

  - Ouvrez l'IDE Arduino.
  - Copiez le code suivant, cliquez sur Vérifier pour vérifier les erreurs de syntaxe. Vérifiez qu'il n'y a pas d'erreurs, et vous pouvez téléverser le code.

```Cpp
// Clignotement de la LED
// La LED s'allumera pendant une seconde, puis s'éteindra pendant une seconde
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





Analyse du code


```cpp
setup(){
}
```

La fonction `setup()` est appelée lorsque le programme démarre. Utilisez-la pour initialiser les variables, les modes de broches, commencer à utiliser des bibliothèques, etc. La fonction `setup()` ne s'exécute qu'une seule fois, après chaque mise sous tension ou réinitialisation de la carte Arduino.

```cpp
loop(){
}
```

Après avoir créé une fonction `setup()`, qui initialise et définit les valeurs initiales, la fonction `loop()` fait précisément ce que son nom suggère, et boucle de manière consécutive, permettant à votre programme de changer et de réagir. Utilisez-la pour contrôler activement la carte Arduino.

```cpp
int ledPin = 4;
```

**Description :**

Convertit une valeur en type de données `int`.

**Syntaxe :**

int(**x**) ou (int)**x** (conversion de type de style C)

**Paramètres :**

**x**: une valeur. Types de données autorisés : n'importe quel type.

Affecte la valeur 4 de type `int` à la variable nommée ledPin.

```cpp
pinMode(ledPin, OUTPUT);
```

**Description :**

Configure la broche spécifiée pour fonctionner en tant qu'entrée ou sortie. Consultez la page des broches numériques pour plus de détails sur les fonctionnalités des broches.

À partir d'Arduino 1.0.1, il est possible d'activer les résistances de pull-up internes avec le mode `INPUT_PULLUP`. De plus, le mode `INPUT` désactive explicitement les résistances de pull-up internes.

**Syntaxe :**

pinMode(**pin, mode**)

**Paramètres :**

**pin** : le numéro de broche Arduino pour définir le mode.

**mode** : `INPUT`, `OUTPUT` ou `INPUT_PULLUP`.

Configuration de la broche ledPin en mode sortie.

```cpp
digitalWrite(ledPin, HIGH);
```

**Description :**

Écrit une valeur `HIGH` ou `LOW` sur une broche numérique.

Si la broche a été configurée en tant que sortie avec pinMode(), sa tension sera réglée sur la valeur correspondante : 5V (ou 3,3V sur les cartes 3,3V) pour `HIGH`, 0V (masse) pour `LOW`.

Si la broche est configurée en tant qu'entrée, digitalWrite() activera (HIGH) ou désactivera (LOW) la résistance de pull-up interne sur la broche d'entrée. Il est recommandé de définir le pinMode() sur `INPUT_PULLUP` pour activer la résistance de pull-up interne. Consultez le tutoriel sur les broches numériques pour plus d'informations.

Si vous ne définissez pas le pinMode() sur OUTPUT et que vous connectez une LED à une broche, lorsque vous appelez digitalWrite(HIGH), la LED peut sembler faible. Sans définir explicitement pinMode(), digitalWrite() aura activé la résistance de pull-up interne, qui agit comme une résistance de limitation de courant importante.

**Syntaxe :**

digitalWrite(**pin, valeur**)

**Paramètres :**

**pin** : le numéro de broche Arduino.

**valeur** : `HIGH` ou `LOW`.

Lorsque nous définissons ledPin en tant que sortie, HIGH signifie envoyer un niveau haut à la broche, la LED s'allume.

```cpp
digitalWrite(ledPin, LOW);
```

Lorsque nous définissons la LED en tant que sortie, LOW signifie envoyer un niveau bas à la broche, la LED s'éteint.

```cpp
delay(1000);
```

**Description:**

Met en pause le programme pendant la durée spécifiée en millisecondes en tant que paramètre. (Il y a 1000 millisecondes dans une seconde.)

**Syntaxe:**

delay(**ms**)

**Paramètres :**

**ms** : le nombre de millisecondes à mettre en pause. Types de données autorisés : unsigned long.

Met le programme en pause pendant 1000ms (1s).

**Effet de démonstration et résultat de l'impression série :**

Le module LED sera allumé pendant 1 seconde, puis éteint pendant 1 seconde.

**Ajustement de la luminosité de la LED :**

<div>
  <div align="center"><img src="https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/LED-res.jpeg" /></div>
  <br />
</div>


Sur le module Grove LED, il y a un **potentiomètre variable qui peut être ajusté à l'aide d'un tournevis.** Tournez-le pour rendre la LED plus lumineuse!


Guide de dépannage


Si les modules sont détachés de la carte. Utilisez un câble Grove pour connecter le **Grove LED** à l'interface numérique **D4** du Seeeduino Lotus.  


### Leçon 2 : Appuyer sur le bouton pour allumer la LED

La première chose que nous devons savoir est que l'entrée du bouton est un signal numérique, et il n'y a que deux états possibles, 0 ou 1, nous pouvons donc contrôler la sortie en fonction de ces deux états.

- **Pratique :** Utilisez le bouton pour allumer et éteindre le module LED

Composants impliqués

  1. Seeeduino Lotus
  2. Grove LED
  3. Grove Button
  4. Câbles Grove (si nécessaire)

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/Button.png)

Connexion matérielle

  - **Connexion du module :**
    - Connexion par défaut via les trous de la carte PCB.
  - Le Seeeduino est ensuite connecté à l'ordinateur via un câble USB.

- **Analyse matérielle** :
  - Entrée : Bouton
  - Contrôle : Seeeduino
  - Sortie : Module LED

Le capteur et la LED utilisent tous deux des signaux numériques, ils doivent donc être connectés à des interfaces numériques.

- **Code logiciel** :
  - Ouvrez l'IDE Arduino.
  - Copiez le code suivant, cliquez sur Vérifier pour vérifier les erreurs de syntaxe. Vérifiez qu'il n'y a pas d'erreurs, puis vous pouvez télécharger le code.

```Cpp
// Bouton pour allumer/éteindre la LED
// Les constantes ne changeront pas. Elles sont utilisées ici pour définir les numéros de broche :
const int buttonPin = 6;    // le numéro de la broche du bouton poussoir
const int ledPin =  4;      // le numéro de la broche de la LED

// Les variables vont changer :
int buttonState = 0;        // variable pour lire l'état du bouton poussoir

void setup() {
  // initialise la broche de la LED en tant que sortie :
  pinMode(ledPin, OUTPUT);
  // initialise la broche du bouton poussoir en tant qu'entrée :
  pinMode(buttonPin, INPUT);
}

void loop() {
  // lit l'état de la valeur du bouton poussoir :
  buttonState = digitalRead(buttonPin);

  // vérifie si le bouton poussoir est enfoncé. S'il l'est, buttonState est HIGH :
  if (buttonState == HIGH) {
    // allume la LED :
    digitalWrite(ledPin, HIGH);
  } else {
    // éteint la LED :
    digitalWrite(ledPin, LOW);
  }
}
```



Analyse du code


```cpp
pinMode(ledPin, OUTPUT);
```

Définit la LED comme unité de sortie.

```cpp
pinMode(buttonPin, INPUT);
```

Définit le bouton comme unité d'entrée.  


```cpp
buttonState = digitalRead(buttonPin);
```

**Description :**

Lit la valeur de la broche numérique spécifiée, soit `HIGH` (élevée) soit `LOW` (bas).

**Syntaxe :**

digitalRead(**pin**)

**Paramètres :**

**pin** : le numéro de la broche Arduino que vous souhaitez lire

Cette fonction est utilisée pour lire les états des broches numériques, soit HIGH (élevée) soit LOW (bas). Lorsque le bouton est enfoncé, l'état est HIGH (élevé), sinon il est LOW (bas).

```cpp
if (buttonState == HIGH) {
  digitalWrite(ledPin, HIGH);
} else {
  digitalWrite(ledPin, LOW);
}
```

**Description :**

La structure if/else permet un contrôle plus précis du flux du code que la simple instruction if, en permettant de regrouper plusieurs tests. Une clause else (si elle existe) est exécutée si la condition dans l'instruction if est fausse. Le else peut être suivi d'un autre test if, de sorte que plusieurs tests mutuellement exclusifs puissent être exécutés en même temps.

Chaque test passe au suivant jusqu'à ce qu'un test vrai soit rencontré. Lorsqu'un test vrai est trouvé, son bloc de code associé est exécuté, puis le programme passe à la ligne suivant la construction if/else entière. Si aucun test ne s'avère vrai, le bloc else par défaut est exécuté, s'il est présent, et définit le comportement par défaut.

Notez qu'un bloc else if peut être utilisé avec ou sans un bloc else de terminaison, et vice versa. Un nombre illimité de ces branches else if est autorisé.



**Syntaxe :**

```cpp
if (condition1) {
  // faire chose A
}
else if (condition2) {
  // faire chose B
}
else {
  // faire chose C
}
```

L'utilisation de l'instruction est la suivante : si l'expression logique entre parenthèses est vraie, exécutez l'instruction entre accolades après **if**, sinon exécutez l'instruction entre accolades après **else**. Si l'état du bouton est haut, la broche de la LED produit un niveau haut et allume la LED, sinon éteint la LED.

**Effet de démonstration et résultat de l'impression série :**

Appuyer sur le bouton allumera le module LED.

Guide de connexion

Utilisez un câble Grove pour connecter la LED Grove à l'interface numérique **D4** de Seeeduino Lotus. Connectez le bouton Grove à l'interface numérique **D6**.






### Leçon 3 : Contrôler la fréquence du clignotement

Dans la dernière section, nous avons étudié que le bouton n'a que deux états, l'état ON/OFF correspondant à 0V et 5V, mais en pratique, nous avons souvent besoin de plusieurs états, pas seulement 0V et 5V. Ensuite, vous devez utiliser un signal analogique ! Le potentiomètre rotatif est un exemple classique qui utilise un signal analogique.

Informations de base :

- **Qu'est-ce qu'un signal analogique**

**Signaux analogiques :** Les signaux varient continuellement dans le temps et la valeur, et l'amplitude, la fréquence ou la phase du signal change continuellement à tout moment, comme le signal sonore diffusé actuellement, ou le signal d'image, etc. Le signal analogique a une onde sinusoïdale et une onde triangulaire, etc. Les broches analogiques de votre microcontrôleur peuvent avoir une tension entre 0V et 5V qui est mappée dans une plage entre 0 et 1023, où 1023 est mappé comme 5V et 512 est mappé comme 2,5V, etc.

![Alt text](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/analog.png)



Composants impliqués
  1. Seeeduino Lotus
  2. Grove LED
  3. Grove Rotary Switch
  4. Câbles Grove (si nécessaire)

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/rotary.png)



Connexion matérielle
  - **Connexion du module :**
    - Connexion par défaut via un trou de la carte PCB.
  - Ensuite, le Seeeduino est connecté à l'ordinateur via un câble USB.

- **Analyse matérielle :**

  - Entrée : Potentiomètre rotatif
  - Contrôle : Seeeduino Lotus
  - Sortie : Module LED

L'entrée est un signal analogique, donc elle est connectée à l'interface de signal analogique, le module LED est connecté à l'interface de signal numérique.


Logiciel

  - Ouvrez l'IDE Arduino.
  - Copiez le code suivant, cliquez sur Vérifier pour vérifier les erreurs de syntaxe. Vérifiez qu'il n'y a pas d'erreurs, puis vous pouvez télécharger le code.

```Cpp
// Contrôle de la LED par le potentiomètre rotatif
int rotaryPin = A0;    // sélectionne la broche d'entrée pour le potentiomètre rotatif
int ledPin = 4;      // sélectionne la broche pour la LED
int rotaryValue = 0;  // variable pour stocker la valeur provenant du potentiomètre rotatif

void setup() {
  // declare the ledPin as an OUTPUT:
  pinMode(ledPin, OUTPUT);
  pinMode(rotaryPin, INPUT);
}

void loop() {
  // lire la valeur du capteur :
  rotaryValue = analogRead(rotaryPin);
  // allumer la broche ledPin :
  digitalWrite(ledPin, HIGH);
  // arrêter le programme pendant <sensorValue> millisecondes :
  delay(rotaryValue);
  // éteindre la broche ledPin :
  digitalWrite(ledPin, LOW);
  // arrêter le programme pendant <sensorValue> millisecondes :
  delay(rotaryValue);
}
```



Analyse du code

```cpp
int rotaryPin = A0;    // sélectionne la broche d'entrée pour le potentiomètre rotatif
int ledPin = 4;      // sélectionne la broche pour la LED
```
**Description :**

Vous pouvez constater que nous définissons rotatePin et ledPin de différentes manières. Cela est dû au fait que le potentiomètre rotatif génère un signal analogique, tandis que la LED est contrôlée par un signal numérique.

Pour **définir une broche analogique**, utilisez A + le numéro de la broche (par exemple, `A0`).

Pour **définir une broche numérique**, utilisez simplement le numéro de la broche (par exemple, `4`).

```cpp
rotaryValue = analogRead(rotaryPin);
```

**Description :**

Lit la valeur de la broche analogique spécifiée. Les cartes Arduino contiennent un convertisseur analogique-numérique multicanal sur 10 bits. Cela signifie qu'il va mapper les tensions d'entrée entre 0 et la tension d'alimentation (5V ou 3.3V) en valeurs entières entre 0 et 1023. Sur une Arduino UNO, par exemple, cela donne une résolution entre les lectures de : 5 volts / 1024 unités, soit 0,0049 volts (4,9 mV) par unité.

**Syntaxe :**

analogRead(**pin**)

**Paramètres :**

**pin** : le nom de la broche d'entrée analogique à lire (A0 à A5 sur la plupart des cartes).

**Renvoie :** La lecture analogique sur la broche. Bien qu'elle soit limitée à la résolution du convertisseur analogique-numérique (0-1023 pour 10 bits ou 0-4095 pour 12 bits). Type de données : int.

Cette fonction est utilisée pour lire la valeur des broches analogiques (la position du capteur rotatif), la plage de valeurs est : 0 ~ 1023.

```cpp
delay(rotaryValue);
```

Fonction de retard : la durée en millisecondes du retard est la valeur entre parenthèses. Comme la valeur est la valeur du signal analogique de la broche du potentiomètre en cours de lecture, le temps de retard peut être contrôlé par le potentiomètre.

**Effet de démonstration et résultat de l'impression série :**

Tourner le potentiomètre modifiera la fréquence du clignotement de la LED.

Guide de connexion

Utilisez un câble Grove pour connecter la LED à l'interface numérique **D4** du Seeeduino Lotus, et un câble Grove pour connecter le commutateur rotatif Grove à l'interface de signal analogique **A0**.

### Leçon 4 : Faire sonner le buzzer

Tout comme le module LED, le buzzer est également un module de sortie qui produit un son de bip. Cela peut être utilisé dans de nombreuses situations à des fins d'indication. Apprenons comment générer du son en utilisant le buzzer !

Informations de base :

- **Quelle est la différence entre un buzzer actif et un buzzer passif**

Il existe deux types de buzzers, l'un est actif et l'autre est passif. Les buzzers actifs et passifs sont utilisés pour produire du son dans les appareils électroniques.

Le **buzzer actif** possède une source d'oscillation interne qui fait retentir le buzzer dès que l'alimentation est appliquée. Les buzzers actifs sont largement utilisés dans les ordinateurs, les imprimantes, les photocopieurs, les alarmes, les jouets électroniques, l'électronique embarquée dans les voitures, les téléphones, les minuteries et autres dispositifs sonores de produits électroniques.

Un **buzzer passif** n'a pas de source d'oscillation interne et doit être piloté par **une onde carrée** et **une fréquence différente**. Il agit comme un haut-parleur électromagnétique, et le signal d'entrée changeant produit du son, plutôt qu'une tonalité automatique.

 <div align="center"><img width={500} src="https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/buzzer-ap.jpg" /></div>


Dans ce kit, le **Grove-Buzzer est un buzzer passif** qui nécessite un signal AC pour le contrôler. Cela nous amène alors à la question suivante, comment générer une onde carrée (signaux AC) avec Arduino ! Eh bien, une façon facile est d'utiliser la modulation de largeur d'impulsion (PWM).

- **Qu'est-ce que le PWM**

La **modulation de largeur d'impulsion, ou PWM** en anglais, est une technique permettant d'obtenir des résultats analogiques avec des moyens numériques. Le contrôle numérique est utilisé pour créer une onde carrée, un signal basculant entre l'état allumé et éteint. Ce motif allumé-éteint peut simuler des tensions entre l'état allumé complet (5 volts) et éteint (0 volt) en modifiant la proportion du temps pendant lequel le signal est allumé par rapport au temps pendant lequel le signal est éteint. La durée de l'état allumé est appelée la largeur d'impulsion. Pour obtenir des valeurs analogiques variables, vous modifiez, ou modulez, cette largeur d'impulsion. Si vous répétez rapidement ce motif allumé-éteint, le résultat est similaire à un signal de tension constante entre 0 et 5 volts en tant que signal AC. *Référence : [Arduino](https://www.arduino.cc/en/tutorial/PWM)*. Ce signal PWM peut ensuite être utilisé pour contrôler facilement le buzzer passif.

Pour générer des signaux PWM avec Arduino, vous pouvez utiliser **`analogWrite()`**, contrairement à l'utilisation de `digitalWrite()` pour générer des signaux DC.

Il y a six broches numériques sur votre Seeeduino qui sont marquées par le symbole "~", ce qui signifie qu'elles peuvent envoyer un signal PWM : 3, 5, 6, 9, 10, 11. Elles sont appelées broches PWM.

Composants impliqués

  1. Seeeduino Lotus
  2. Grove Buzzer
  3. Câble Grove (si nécessaire)

![](https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/Buzzer.png)



Connexion matérielle

  - **Connexion du module**
    - Connexion par défaut via le trou de la carte PCB.
  - Connectez le Seeeduino à l'ordinateur via le câble USB.

Code logiciel

  - Ouvrez l'IDE Arduino.
  - Copiez le code suivant, cliquez sur Vérifier pour vérifier les erreurs de syntaxe. Vérifiez qu'il n'y a pas d'erreurs, et vous pouvez télécharger le code.

```Cpp
int BuzzerPin = 5;

void setup() {
  pinMode(BuzzerPin, OUTPUT);
}

void loop() {
  analogWrite(BuzzerPin, 128);
  delay(1000);
  analogWrite(BuzzerPin, 0);
  delay(0);
}
```

Analyse de code

```cpp
analogWrite(BuzzerPin, 128);
```

**Description :**

Écrit une valeur analogique (onde PWM) sur une broche. Peut être utilisé pour allumer une LED à différentes intensités lumineuses ou pour contrôler la vitesse d'un moteur. Après un appel à analogWrite(), la broche générera une onde rectangulaire stable avec le rapport cyclique spécifié jusqu'au prochain appel à analogWrite() (ou un appel à digitalRead() ou digitalWrite()) sur la même broche.

**Syntaxe :**

analogWrite(**broche, valeur**)

**Paramètres:**

**broche**: la broche Arduino sur laquelle écrire. Types de données autorisés : int.

**valeur**: le rapport cyclique : entre `0` (toujours éteint) et `255` (toujours allumé). Types de données autorisés : int.

Écrit une valeur analogique (onde PWM) sur le Buzzer.

**Effet de démonstration et résultat de l'impression série:**

Le Buzzer émet un bip.

Guide de connexion

Utilisez un câble Grove pour connecter le Buzzer Grove à l'interface numérique **D5** du Seeeduino Lotus.

-----

Utilisation de la PWM

Maintenant que nous avons appris à utiliser la PWM, en plus de l'utiliser pour contrôler le buzzer passif, nous pouvons également l'utiliser pour contrôler la vitesse d'un moteur et **l'intensité lumineuse des LED**, etc.

Comme l'indique le diagramme ci-dessous, utilisez `analogWrite()` pour générer des ondes PWM. Plus le pourcentage du rapport cyclique est élevé, plus la LED est lumineuse.

<div align="center"><img src="https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/PWM-LED.png" /></div>


Cependant, le module LED sur le kit débutant Grove ne peut pas être directement contrôlé par PWM, car le module LED est connecté à D4, et comme mentionné ci-dessus, les broches PWM sont 3, 5, 6, 9, 10, 11, et la broche 4 n'est pas une broche PWM. Si vous souhaitez contrôler la LED avec PWM, vous devez la déconnecter et utiliser le câble Grove pour la connecter au port Grove avec une fonction PWM.

Par exemple, connectons **Grove-LED à D3 en utilisant un câble Grove**:

!!!Note
  D3 est également interconnecté au capteur de température et d'humidité Grove, et donc cet exemple ne peut pas être utilisé avec le capteur de température et d'humidité Grove en même temps.

<div align="center"><img src="https://files.seeedstudio.com/wiki/Grove-Beginner-Kit-For-Arduino/img/pwmled-connect.png" /></div>

```cpp
int LED = 3; // Connexion du câble de la LED à D3
int Potentiometer = A0;

void setup() {
  pinMode(LED, OUTPUT);
  pinMode(Potentiometer, INPUT);
}

void loop() {
  int potentioValue, Value;
  potentioValue = analogRead(Potentiometer);
  Value = map(potentioValue, 0, 1023, 0, 255); // Mappage de la valeur du potentiomètre à la valeur du signal PWM
  analogWrite(LED, Value);
}
```

**Compilez et téléversez** le code, vous devriez pouvoir régler la luminosité de la LED en utilisant des signaux PWM !

Analyse du code

```cpp
Value = map(potentioValue, 0, 1023, 0, 255);
```

**Description:**

Remappe un nombre d'une plage à une autre. C'est-à-dire, une valeur de **fromLow** serait mappée à **toLow**, une valeur de **fromHigh** à **toHigh**, des valeurs intermédiaires à des valeurs intermédiaires, etc.

Ne contraint pas les valeurs à l'intérieur de la plage, car les valeurs hors de la plage sont parfois intentionnelles et utiles. La fonction `constrain()` peut être utilisée avant ou après cette fonction, si des limites aux plages sont souhaitées.

Notez que les "bornes inférieures" de chaque plage peuvent être plus grandes ou plus petites que les "bornes supérieures", de sorte que la fonction `map()` peut être utilisée pour inverser une plage de nombres, par exemple :

**y = map(x, 1, 50, 50, 1);**

La fonction gère également bien les nombres négatifs, de sorte que cet exemple

**y = map(x, 1, 50, 50, -100);**

est également valide et fonctionne bien.

La fonction `map()` utilise des calculs entiers, elle ne générera donc pas de fractions, même si les calculs pourraient l'indiquer. Les restes fractionnaires sont tronqués et ne sont ni arrondis ni moyennés.

**Syntaxe :**

map(**valeur, fromLow, fromHigh, toLow, toHigh**)

**Paramètres :**

**valeur** : le nombre à mapper.

**fromLow** : la limite inférieure de la plage actuelle de la valeur.

**fromHigh** : la limite supérieure de la plage actuelle de la valeur.

**toLow** : la limite inférieure de la plage cible de la valeur.

**toHigh** : la limite supérieure de la plage cible de la valeur.

Mapping du signal analogique du capteur de potentiomètre (0 à 1023) à l'intensité lumineuse de la LED (0 à 255).

**Effet de démonstration et résultat de l'impression série :**

Ajustez le potentiomètre pour ajuster la luminosité de la LED.

En résumé, lorsque vous souhaitez utiliser la fonction PWM, assurez-vous de sélectionner les broches avec le symbole "~" devant leur nom.

### Lesson 5:  Making an Light Induct LED



