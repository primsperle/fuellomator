# fuellomator
Halbautomatischer Gegendruckabfüller für Bier mit Arduino Uno

Test Steuerung: https://youtu.be/0JZCbqLwJvY (noch ohne CO2-Spülung am Ende)

![alt tag](https://github.com/primsperle/fuellomator/blob/master/Aufbau.jpg)

Basis: Gegendruckabfüller aus Heizung/Sanitärteilen mit z.B. 1/4" Anschlüssen für CO2 und Bier, erhältlich in Hobbybrauershops oder Selbstbau nach bekannten Anleitungen (http://braumagazin.de/article/soda-kegs/  http://hobbybrauer.de/modules.php?name=eBoard&file=viewthread&tid=17245)

Funktionsweise/Ablauf:

-Tastendruck zum Start des Abfüllvorgangs, Magnetventil "CO2" öffnet für 4 Sekunden,

-Vorspannen einer Flasche mit CO2 für 4 Sekunden,

-CO2-Ventil schließt, Bierventil öffnet,

-Füllvorgang mit Bier gestoppt durch Füllstandssensor (Digitaleingang Arduino mit Pullup),




WIE?

-CO2 und Bierleitung gesteuert durch Magnetventile über Relaisplatine an Digitalausgängen Arduino

-Füllgeschwindigkeit geregelt über manuelles CO2-Ablassventil,

-Anzeigeausgabe über 16x2 LCD, jeweiliger Status wird angezeigt, zusätzlich Anzeige über 2 LEDs

Teile: 

-Arduino UNO Rev3 oder Clone

-I2C 16x2 LCD mit Backpack

http://www.sunfounder.com/wiki/index.php?title=I%C2%B2C_LCD1602



-China Relaisplatine (2-Kanal) 

-2 Magnetventile 12V, z.B. 1/4" mit IQS schnellverbindern

-Taster

-2 LED (z.B. grün für Meldung "Flasche voll" und rot (Auch  Blink-LED) für "Füllvorgang"

-10k Pullup bzw. Pulldown Widerstände 




Aufbau: 

![alt tag](https://github.com/primsperle/fuellomator/blob/master/fuellomator_Schema.jpg)



erforderliche Libraries:

-Wire.h

-LiquidCrystal_I2C.h

download: http://www.sunfounder.com/wiki/index.php?title=File:LiquidCrystal_I2C.zip


