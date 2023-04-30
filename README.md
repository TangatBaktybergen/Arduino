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
  1. die erforderliche Spannungsversorgung von 5V herstellen
  2. einen Kommunikationskanal zwischen Rechner und Arduino-Boardbereitstellen

Die Power-Anschluss wird benötigt, um das Arduino-Board nach der Programmierung unabhängig vom Rechner zu machen, über den es zuvor programmiert wurde. 
Die vorgeschlagene Spannung sollte sich im Bereich von 7V bis 12V DC bewegen

* Die Ein- und Ausgänge

Es ist eine Durchnummerierung von 0 bis 13 zu erkennen, wobei machen Nummern eine Schlangenlinie - auch Tilde genannt - voransteht. Eben so gibt es Zwei Pins, an denen sich die Zusatzinformation RX und TX befinden. Sie sollten im Normalfall nicht zur Ansteurung verwendet werden, da sie von der seriellen Schnittstelle standardmäßig belegt sind. 

* PWM-Signal

Eine PWM-Signal besitzt eine konstante Frequenz mit einer konstanten Spannung. Was jedoch variieren kann, ist der sogenannte Tastgrad. Wenn die Frequenz f gleich bleibt, dass ebenfallsdie Periodendauer T konstant ist. Die Impulsedauer kann sich ändern, Je breiter der Impulsquasi größere Fläche -, desto größer ist auch die Energie.

* Der Flash-Speicher

Der Flash-Speicher speichert der Sketch ( die Aufgaben ) für den Mikrocontroller. Wird der Arduino von der Spannungsversorgung getrennt und ist somit stromlos, dann bleibt der Sketch resistent im Speicher.

* Das SRAM 

Die Abkürzung von SRAM lautet Static Random Access Memory. Wird ein Sketch zum Beispiel zur Verarbeitung von Messwerten benötigt, dann müssen diese Werte in irgendeiner Form innerhalb des Mikrocontrollers abgelegt werden.Dazu benutzt man sogenannte Variablen, die als Platzhalter fungieren. Es handelt sich um spezielle Speicherbereiche sind jedoch flüchtig, was bedeutet, dass sie ihre Informationen nach dem Abschalten der Spannungsversorgung verlieren. 

* Das EEPROM 

Die Abkürzung EEPROM steht für Electrically Erasable Programmable Read-Only Memory.Es handelt sich wie beim Flash-Speicher. Es ist benutzt um wichtige Daten wie zum b. Messwerte permanent zu speichern. Die Schreibzugriffe auf diesen Speicherbereich ist begrenzt. Die maximalen Screib- und Löschrogänge sind offiziell mit einem Wert von 100 000 angegeben. 
