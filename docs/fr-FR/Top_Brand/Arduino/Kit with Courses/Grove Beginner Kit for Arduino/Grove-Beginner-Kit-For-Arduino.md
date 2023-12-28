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





### Lesson 2: Pressing Button to Light Up LED
