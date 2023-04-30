# Arduino
Die Beschreibung von ATmega328 Mikrocontroller , die das Hertz von Arduino UNO ist. 

| Bezeichnung             | Detail       |
| ------------------      | ------------ |
| Mikrocontroller         | ATmega328    | 
| Arbeitsspannung         | 5V           |
| Eingangsspannung        | 7V to 12 V   |
| Eingangsspannung(Limit) | 6V to 20V    |
| Digitale I/O-Pins       | 14(6 für PWM)|
| Analoge Engänge         | 6            |
| DC Strom pro I/O-Pin    | 40mA         |
| DC Storm für 3.3V Pin   |  50mA        |
| Flash-Speicher          | 32KByte      |
| SRAM                    | 2KByte       |
| EEPROM                  | 1KByte       |
| Taktrate                | 16MHz        |


* Was genau ist ein Bootloader? 
Ein Bootloader ist ein kleines Programm, das in einem bestimmten Bereich des Flash-Speichers auf dem Mikrocontrollerboard seinen Platz findet und für das Laden des eigentlichen Programms verantwortlich ist. Normalerweise wird ein Mikrocontroller über zusätzliche Hardware, zum Beispiel einen ISP-Programmer, mit dem Arbeitsprogramm versehen. Durch den Bootloader enfällt diese Notwendigkeit. Nach dem erfolgreichen Übertragen des Arbeitsprogramms in den Arbeitsspeicher des Controllers wird es unmittelbar zur Ausführung gebracht.

* Die Spannungsversorgung 
Wenn wir mit dem Arduino arbeiten oder ihn programmieren, dann ist natürlich eine USB-Verbindung zum Rechner notwending.Diese Verbindung hat zwei Aufgaben:
*  die erforderliche Spannungsversorgung von 5V herstellen
*  einen Kommunikationskanal zwischen Rechner und Arduino-Boardbereitstellen

