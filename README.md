# Mikrofonumschalter

## Idee:

Mit Hilfe von drei Elgato Streamdeck Minis soll eine t.racks 8x8 Matrix über einen Raspberry Pi und die RS232 Schnittstelle gesteuert werden. Die Übermittlung von USB auf RS232 wird ein Python Skript übernehmen.

Die Hierfür notwendigen Befehle sind in der [Betriebsanleitung des Herstellers](https://images.static-thomann.de/pics/atg/atgdata/document/manual/490507_c_490507_r1_de_online.pdf) ab Seite 52 aufgelistet. Raspberry Pi und weitere Hardware sollen dann in einem 1HE Rack für eine Festinstallation verbaut werden. Da eine Höheneinheit eine maximale Höhe von 44mm zulässt kann der Raspberry Pi kein aktiv kühlendes Gehäuse besitzen. Darum werden in die Vorder- und Rückseite des Gehäuses Schlitze gefräst, hinter die je ein Lüfter geschraubt wird. Somit kann Luft durch das Gehäuse am Raspberry Pi ziehen und diesen kühlen.

## Benötigte Hardware:

Grundsätzlich sind zwei Varianten denkbar, welche sich nicht in der Grundfunktionalität jedoch in Ausstattung und Komfort unterschieden.

### Variante 1 (Basic):

- 1x [**Raspberry Pi 4B**](https://amazon.de/dp/B07TD42S27/) 
- 1x [**SD-Karte**](https://www.amazon.de/dp/B06XYHN68L/) (Für das Betriebssystem, darum braucht es eine zuverlässige Karte)
- 1x **[Gehäuse](https://www.amazon.de/dp/B07XRL1VNQ/)** (Für passive Kühlung)
- 1x **[Gehäuselüfer](https://www.amazon.de/dp/B07ZBRGC5K/)** (Da ein aktiv lüftendes Gehäuse aufgrund der Höhe von 44mm des Racks nicht möglich ist.)
- 1x **[Netzteil](https://www.amazon.de/dp/B07DC97TMM/)** für den Raspberry Pi (3A werden benötigt um Lüfter ansteuern zu können)
- 1x **[3m USB 2.0 Kabel](https://www.amazon.de/dp/B00WHZ7GBW/)**
- 2x **[2m USB 2.0 Kabel](https://www.amazon.de/dp/B00WHZ7AGS/)**
- 1x **[RS232 Board](https://www.amazon.de/dp/B0107Y3Z3W/)**
- 1x **[RS232 Kabel](https://www.amazon.de/dp/B00A6GIUZA/)**
- **[Kabelschlauch](https://www.amazon.de/dp/B09TNL7PCK/)** (um das Kabelbündel an der Gehäuserückseite durch ein Loch ausführen zu können)

Diese Variante setzt eine Konfiguration und Wartung über WLAN oder LAN voraus, da keine weiteren Anschlüsse für HDMI und USB verfügbar sind. Alle Kabel werden durch ein Loch in der Gehäuserückseite ausgeführt und sind nicht absteckbar.



### Variante 2:

Zusätzlich zu den in Variante 1 gelisteten Artikeln wird Folgendes benötigt:

- 1x **[HDMI Feed Through](https://www.amazon.de/dp/B004E8A77U/)**
- 1x [**RJ45 Feed Through**](https://www.amazon.de/dp/B004E8DKBA/)
- 5x **[USB 2.0 Feed Through](https://www.amazon.de/dp/B003VSXQVI/)**
- 1x [**USB-C Feed Through**](https://www.amazon.de/-/en/dp/B076954GFC/)
- 1x [**USB-C 0.5m Verlängerung**](https://www.amazon.de/dp/B074K318JK/)
- 5x [**USB 2.0 0.5m Verlängerung**](https://www.amazon.de/dp/B00WHZ7N60/)
- 1x [**Micro HDMI zu HDMI Adapter**](https://www.amazon.de/dp/B00B2HORKE/)
- 1x [**0.5m HDMI Kabel**](https://www.amazon.de/dp/B08R425QQ3/) 
- 1x [**USB 2.0 HUB**](https://www.amazon.de/dp/B00L2442H0/)

Die Idee ist, dass an der Rückseite des Racks alle Kabel an- und abgesteckt werden. Dadurch wäre das Rack an sich handlicher und Kabel könnten gewechselt/getauscht werden, ohne das Gehäuse öffnen zu müssen. Wahlweise kann auf den RJ45-, HDMI-, 2x USB- Feed Tough und den USB HUB verzichtet werden, falls eine Wartung des Pis nicht oder nur in seltenen Fällen vorhergesehen ist.

Der Raspberry Pi wird in der Mitte des Gehäuses befestigt und mit den 0.5m Patchkabeln an die Rückseiten der Feed Troughs angeschlossen. Von außen können nun nach Bedarf unterschiedliche Kabel (z.B. bei Defekt) getauscht werden.



