# SqueezeboxRadioHwWiFi6Fix
Squeezebox Radio WiFi6 hardware based fix - Installation of a WiFi LAN bridge

# Squeezebox Radio - Einbau WiFi-LAN-Bridge 
## Warum?
Seit der Einführung von WiFi6 gibt es Probleme mit dem SqueezeboxRadio.
Der eingebaute WiFi-Chip scheint sich in unregelmäßigen Abständen aufzuhängen. Ein Neustart ist notwendig, um die Verbindung neu aufzubauen. Laut Beobachtungen von Usern des Squeezebox-Forums kommt dies sogar vor, wenn man selbst kein WiFi6 betreibet, es reicht wohl, wenn ein fremdes WiFi Netz in der Gegend WiFi6 verwendet.

Siehe Thread: https://www.squeezebox-forum.de/viewtopic.php?t=3990

Laut einigen Usern soll die Community-Firmware Version 8.5.0-r16962 das Problem lösen. Vermutlich wird in dieser Version der WiFi-Chip bei einem Abbruch neu initialisiert. Dies passiert solange der Buffer genügend gefüllt ist, um eine Unterbrechung zu verhindern. (Das ist nur meine Vermutung der Funktionsweise!)

Ich habe diesen Lösungsansatz nicht weiterverfolgt, da für mich die unten beschriebene Hardware-Lösung einfach einzubauen ist und die WiFi-LAN-Bridge auf moderne WiFi-Empfangstechnologie setzt.

Laut einem User soll wohl die oben erwähnte Community-Firmware Version auch weiterhin Probleme haben, insbesondere wenn man ein FRITZ!box Mesh mit Repeatern betreibet.

Siehe: https://www.squeezebox-forum.de/viewtopic.php?p=28082#p28082


## Haftung
Keine Ahnung, warum ich das hier schreibe, der XMV* müsste einem das Folgende eigentlich selbst sagen:

Ich übernehme keinerlei Haftung für Schäden am SqueezeboxRadio, am Werkzeug noch übernehme ich Haftung für Schäden an Leib und Leben irgendwelcher Personen oder Tiere, ich übernehme auch keine Haftung für Schäden am Rest des Universums. Jede und jeder die bzw. der dieser Anleitung folgt, ist für sein bzw. ihr Handeln selbst verantwortlich. Wenn das für Sie nicht ok ist, dann verlassen Sie jetzt diese Seite.

(* XMV = Xunder Menschen Verstand)


## Support
Ich werde nur Support leisten, wenn es mir meine freie Zeit erlaubt und ich gerade Bock darauf habe.


## Material
-	WiFi-LAN-Bridge
  Hersteller: TP-Link
  Bezeichnung: 300Mbps Wireless N Nano Router
  Typ: TL-WR802N
  Link: https://www.tp-link.com/de/home-networking/wifi-router/tl-wr802n/
-	rote und schwarze flexible Litze
-	TX8 Schraubendreher
-	TX10 Schraubendreher
-	Plektrum (oder anderes dünnes Kunststoffteil)
-	Feiner Lötkolben und Lötzinn
-	Ggf. Kopflupe
-	Heißkleber
-	Kleine Bohrmaschine, um das Loch für die Versorgungslitzen zu bohren
-	Klebeband


# Umbauanleitung

## 1. Abnehmen der Lautsprecherblende
Hierbei kann ein Plektrum sehr hilfreich sein.

![Abnehmen der Lautsprecherabdeckung](./pics/001.png)

![Abnehmen der Lautsprecherabdeckung](./pics/002.png)

![Abnehmen der Lautsprecherabdeckung](./pics/003.png)

## 2. Gummiteil an der Netzwerkbuche entfernen
Dies lässt sich mit einem Schlitzschraubendreher vorsichtig heraushebeln.

![Gummiteil Netzwerkbuchse ausbauen](./pics/004.png)

## 3.	Zwei TX8 Schrauben entfernen
 
![TX8 Schrauben](./pics/005.png)

## 4. Bedienteil nach links schieben
Dadurch löst es sich aus der rechten Arretierung.
   
![TX8 Schrauben](./pics/006.png)

![TX8 Schrauben](./pics/007.png)

## 5. Steckverbinder Lautsprecherkabel lösen

![TX8 Schrauben](./pics/008.png)

## 6. Steckverbinder der externen Spannungsversorgung lösen

![TX8 Schrauben](./pics/009.png)

## 7. Sechs TX10 Schrauben lösen

![TX8 Schrauben](./pics/010.png)

## 8. Gehäusehälften auseinanderziehen
Da die Dichtung gut haftet, geht dies beim ersten Öffnen relativ schwer. 
Wenn man das Batteriefach geöffnet hat, kann man von innen drücken.

![TX8 Schrauben](./pics/011.png)

## 9. Mit einem dünnen Bohrer an der im Bild gekennzeichneten Position ein Loch bohren. 
Dieses wird für die Litzen der 3,3 Volt Versorgung benötigt.

![TX8 Schrauben](./pics/012.png)

![TX8 Schrauben](./pics/013.png)

![TX8 Schrauben](./pics/014.png)

## 10. Öffnen der WiFi-LAN-Bridge
Das Gehäuse der WiFi-LAN-Bridge ist nur geclipst. 
Mit einem entsprechend dünnen Werkzeug muss zwischen die beiden Gehäusehälften gefahren werden und dann die beiden Hälften auseinander gehebelt werden.
Auf der Rückseite des Gehäuses sind die Zugangsdaten auf einem Label aufgedruckt. Es empfiehlt sich, diese Daten zu notieren, oder das Label abzulösen und auf das SqueezeboxRadio zu übertragen.

![TX8 Schrauben](./pics/015.png)

![TX8 Schrauben](./pics/016.png)

![TX8 Schrauben](./pics/017.png)




