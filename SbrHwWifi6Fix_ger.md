[Teslink](SqueezeboxRadioHwWifi6Fix_ger.md)

# SqueezeboxRadioHwWiFi6Fix
Squeezebox Radio WiFi6 hardware based fix - Installation of a WiFi LAN bridge

# Squeezebox Radio - Einbau WiFi-LAN-Bridge 
## Warum?
Seit der Einführung von WiFi 6 gibt es Probleme mit dem Squeezebox Radio. Der eingebaute WiFi-Chip scheint sich in unregelmäßigen Abständen aufzuhängen. Ein Neustart ist notwendig, um die Verbindung neu aufzubauen. Laut Beobachtungen von Nutzern des Squeezebox-Forums tritt dies sogar dann auf, wenn man selbst kein WiFi 6 betreibt. Es reicht offenbar aus, wenn ein fremdes WiFi-Netz in der Umgebung WiFi 6 verwendet.

Siehe Thread: https://www.squeezebox-forum.de/viewtopic.php?t=3990

Laut einigen Nutzern soll die Community-Firmware Version 8.5.0-r16962 das Problem lösen. Vermutlich wird in dieser Version der WiFi-Chip bei einem Abbruch neu initialisiert. Dies passiert, solange der Puffer genügend gefüllt ist, um eine Unterbrechung zu verhindern. (Das ist nur meine Vermutung zur Funktionsweise!)

Ich habe diesen Lösungsansatz nicht weiterverfolgt, da für mich die unten beschriebene Hardware-Lösung einfach zu implementieren ist und die WiFi-LAN-Bridge auf moderne WiFi-Empfangstechnologie setzt.

Laut einem Nutzer soll auch die oben erwähnte Community-Firmware-Version weiterhin Probleme haben, insbesondere wenn man ein FRITZ!Box-Mesh mit Repeatern betreibt.

Siehe: https://www.squeezebox-forum.de/viewtopic.php?p=28082#p28082


## Haftung
Keine Ahnung, warum ich das hier schreibe – der XMV* müsste einem das Folgende eigentlich selbst sagen:

Ich übernehme keinerlei Haftung für Schäden am Squeezebox Radio, noch für Schäden an Leib und Leben von Personen oder Tieren. Ebenso übernehme ich keine Haftung für Schäden am Rest des Universums, einschließlich des verwendeten Werkzeugs. Jede und jeder, die bzw. der dieser Anleitung folgt, ist für ihr bzw. sein Handeln selbst verantwortlich. Wenn das für Dich nicht in Ordnung ist, verlasse jetzt diese Seite.

Solltest Du noch nie einen Lötkolben in der Hand gehabt haben, lass es bitte sein und lerne erst, zu löten!

(* XMV = Xunder Menschen Verstand)


## Support
Ich werde nur Support leisten, wenn es mir meine freie Zeit erlaubt und ich gerade Bock darauf habe.


## Material
-	WiFi-LAN-Bridge<br>
  Hersteller: TP-Link<br>
  Bezeichnung: 300Mbps Wireless N Nano Router<br>
  Typ: TL-WR802N<br>
  Link: https://www.tp-link.com/de/home-networking/wifi-router/tl-wr802n/<br>
-	rote und schwarze flexible Litze
-	TX8 Schraubendreher
-	TX10 Schraubendreher
-	Plektrum (oder anderes dünnes Kunststoffteil)
-	Feiner Lötkolben und Lötzinn
-	Ggf. Kopflupe
-	Heißkleber
-	Bohrmaschine mit einem dünnem Bohrer (um das Loch für die Versorgungslitzen zu bohren)
-	Klebeband (zum Befestigen der Leitungen im Gehäuse)


# Umbauanleitung


## 1. Abnehmen der Lautsprecherblende
Hierbei kann ein Plektrum sehr hilfreich sein.

![Abnehmen der Lautsprecherabdeckung](./pics/001.png)

![Abnehmen der Lautsprecherabdeckung](./pics/002.png)

![Abnehmen der Lautsprecherabdeckung](./pics/003.png)


## 2. Gummiteil an der Netzwerkbuche entfernen
Dieses lässt sich mit einem Schlitzschraubendreher vorsichtig heraushebeln.

![Gummiteil Netzwerkbuchse ausbauen](./pics/004.png)


## 3.	Zwei TX8 Schrauben entfernen
 
![TX8 Schrauben](./pics/005.png)


## 4. Bedienteil nach links schieben
Dadurch löst es sich aus der rechten Arretierung.
   
![Bedienteil](./pics/006.png)

![Bedienteil](./pics/007.png)


## 5. Steckverbinder Lautsprecherkabel lösen

![Steckverbinder](./pics/008.png)


## 6. Steckverbinder der externen Spannungsversorgung lösen

![Steckverbinder](./pics/009.png)


## 7. Sechs TX10 Schrauben lösen

![TX10 Schrauben](./pics/010.png)


## 8. Gehäusehälften auseinanderziehen
Da die Dichtung gut haftet, geht dies beim ersten Öffnen relativ schwer. 
Wenn man das Batteriefach geöffnet hat, kann man von innen drücken.

![Gehäuse](./pics/011.png)


## 9. Mit einem dünnen Bohrer an der im Bild gekennzeichneten Position ein Loch bohren. 
Dieses wird für die Litzen der 3,3 Volt Versorgung benötigt.

![Loch](./pics/012.png)

![Loch](./pics/013.png)

![Loch](./pics/014.png)


## 10. Öffnen der WiFi-LAN-Bridge
Das Gehäuse der WiFi-LAN-Bridge ist nur geclipst. 
Mit einem entsprechend dünnen Werkzeug muss zwischen die beiden Gehäusehälften gefahren werden und dann die beiden Hälften auseinander gehebelt werden.
Auf der Rückseite des Gehäuses sind die Zugangsdaten auf einem Label aufgedruckt. Es empfiehlt sich, diese Daten zu notieren, oder das Label abzulösen und auf das SqueezeboxRadio zu übertragen.

![WiFi-Bridge](./pics/015.png)

![WiFi-Bridge](./pics/016.png)

![WiFi-Bridge](./pics/017.png)

![WiFi-Bridge](./pics/018.png)


## 11. Elektrische Verbindungen WiFi-LAN-Bridge
Die 3,3 Volt vom Squeezebox Radio werden auf der Platine der WiFi-LAN-Bridge *nach* dem Spannungsregler eingespeist.
Die rote Litze muss hierfür an TP5 angelötet werden. 
Die schwarze Litze für GND wird an einer der beiden Gehäuse-Lötstellen der USB Buchse angelötet. 

Die Litzen werden anschließend mit etwas Heißkleber auf der Leiterplatte fixiert.

![Versorgungsspannung](./pics/019.png)

![Versorgungsspannung](./pics/019a.png)

![Versorgungsspannung](./pics/020.png)


## 12 Einbau WiFi-LAN-Bridge
Die WiFi-LAN-Bridge befindet sich an der linken Seite des Lautsprechers. Mit etwas Heißkleber kann das Modul am Kunststoff des Gehäuses fixiert werden. 
Es ist darauf zu achten, dass der RJ45-Stecker des LAN-Kabels ebenfalls Platz findet. Am besten sollte das Modul mit eingestecktem RJ45-Stecker fixiert werden.

![Einbau](./pics/021.png)


## 13 Leitungen im Gehäuse verlegen
Das LAN-Kabel und die Litzen der 3,3 Volt Versorgung werden wie im folgenden Bild gezeigt im Gehäuse verlegt und mit etwas Klebeband fixiert.

![Leitungen](./pics/022.png)


## 14 Elektrische Verbindungen SqueezeboxRadio Mainboard
Die 3,3 Volt werden am Spannungsregler des Squeezebox Radios abgenommen.
Die rote Litze kann hierfür an den Testpunkt zwischen R240 und C140 angelötet werden.
Die schwarze Litze für GND wird an den Masse-Pin von C35 angelötet.

Die Litzen werden mit etwas Heißkleber auf der Leiterplatte fixiert.

Dieser Abgriff nach dem 3,3-Volt-Regler hat den Vorteil, dass die WiFi-LAN-Bridge beim Abschalten des Squeezebox Radios ebenfalls komplett abgeschaltet wird.
Insbesondere beim Betrieb mit dem eingebauten Akku ist dies von Vorteil.

![Mainboard](./pics/023.png)

![Mainboard](./pics/024.png)

![Mainboard](./pics/025.png)

![Mainboard](./pics/026.png)


## 15 Herausführen des LAN-Kabel
Der Gummieinsatz rund um die Netzwerkbuchse muss etwas eingeschnitten werden, um Platz für das LAN-Kabel freizugeben.

![Mainboard](./pics/027.png)


## 16 Zusammenbau
Der Zusammenbau erfolgt in umgekehrter Reihenfolge zum Öffnen des Gehäuses. Dabei ist darauf zu achten, dass keine der Litzen eingeklemmt wird.


# Viel Erfolg!
written 07.12.2024 by Timo Engelmann
Quelle: https://github.com/FluxPower42/SqueezeboxRadioHwWiFi6Fix/blob/main/SbrHwWifi6Fix_ger.md