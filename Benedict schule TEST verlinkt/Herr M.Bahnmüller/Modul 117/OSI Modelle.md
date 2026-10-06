Ja. Aus **dieser Buchseite** solltest du vor allem **OSI ↔ TCP/IP und die wichtigen Protokolle** lernen.

### 1. OSI-Modell und TCP/IP-Modell

|OSI-Schicht|Name|Gehört bei TCP/IP zu|
|--:|---|---|
|**7**|Application Layer / Anwendung|**Anwendungs-Schicht**|
|**6**|Presentation Layer / Darstellung|**Anwendungs-Schicht**|
|**5**|Session Layer / Sitzung|**Anwendungs-Schicht**|
|**4**|Transport Layer|**Transport-Schicht (TCP)**|
|**3**|Network Layer / Vermittlung|**Internet-Schicht (IP)**|
|**2**|Data Link Layer / Sicherung|**Netzwerk- und Link-Schicht**|
|**1**|Physical Layer / Bitübertragung|**Netzwerk- und Link-Schicht**|
Genau **dieses Format** für alle 7 Schichten:

### OSI-Schicht 1 – Physical Layer / Bitübertragungsschicht

- **Definition:** Regelt die physische Übertragung von Bits über ein Übertragungsmedium.  
- **Aufgaben:** Signalübertragung, Signalregenerierung, Autonegotiation, Autosensing.  
- **Komponenten laut deinem Buch:** Repeater, Hub, Medienkonverter.

###### OSI-Schicht 2 – Data Link Layer / Sicherungsschicht

- **Definition:** Regelt die Übertragung von Frames innerhalb eines lokalen Netzwerks.  
- **Aufgaben:** Switching, MAC-Adressierung, Übertragung von Frames.  
- **Komponenten laut deinem Buch:** Bridge, Switch, Access Point, Netzwerkadapter.

###### OSI-Schicht 3 – Network Layer / Vermittlungsschicht

- **Definition:** Regelt die Weiterleitung von Datenpaketen zwischen verschiedenen Netzwerken.  
- **Aufgaben:** Routing, IPv4-/IPv6-Adressierung, IP-Filterung.  
- **Komponenten laut deinem Buch:** Router, Multilayerswitch (Layer-3-Switch), Paketfirewall.

###### OSI-Schicht 4 – Transport Layer / Transportschicht

- **Definition:** Regelt die Ende-zu-Ende-Übertragung von Daten zwischen Anwendungen.  
- **Aufgaben:** Segmentierung, Fehlerkorrektur mit TCP, Portfilterung.  
- **Komponenten laut deinem Buch:** Layer-4-Switch, Stateful-Inspection-Firewall.  
**Protokolle:** TCP, UDP.

###### OSI-Schicht 5 – Session Layer / Sitzungsschicht

- **Definition:** Regelt die Kommunikationssitzungen zwischen Anwendungen.  
- **Aufgaben:** Aufbau, Steuerung und Beendigung einer Sitzung.  
- **Protokoll laut deiner Unterlage:** RPC.  
- **Komponenten:** In deiner Tabelle sind keine angegeben.

###### OSI-Schicht 6 – Presentation Layer / Darstellungsschicht

- **Definition:** Regelt die Darstellung und Aufbereitung der Daten für Anwendungen.  
- **Aufgaben:** Daten in eine für Anwendungen nutzbare Darstellung bringen.  
- **Komponenten/Protokolle:** In deiner Tabelle sind keine angegeben.

###### OSI-Schicht 7 – Application Layer / Anwendungsschicht

- **Definition:** Stellt Anwendungen Netzwerkfunktionen und Netzwerkdienste zur Verfügung.  
- **Aufgaben laut deinem Buch:** Protokollumsetzung auf Applikationsebene.  
- **Komponenten laut deinem Buch:** Gateway, Proxy, Application-Layer-Firewall.  
- **Protokolle laut deiner Unterlage:** HTTP, HTTPS, FTP, SMTP.

Zum schnellen Auswendiglernen:**  
1 Bits → 2 MAC → 3 IP → 4 TCP/UDP → 5 Sitzung → 6 Darstellung → 7 Anwendung**





**Wichtig:** TCP/IP hat hier **4 Schichten**, OSI hat **7 Schichten**.

### 2. Protokolle – das musst du können

|Protokoll|OSI|Ausgeschrieben|Aufgabe|
|---|--:|---|---|
|**FTP**|**7**|File Transfer Protocol|Dateiübertragung|
|**SMTP**|**7**|Simple Mail Transfer Protocol|E-Mails versenden|
|**HTTP**|**7**|Hypertext Transfer Protocol|Webseiten/HTML übertragen|
|**HTTPS**|**7**|HTTP over SSL/TLS|Verschlüsselte HTTP-Verbindung|
|**RPC**|**5**|Remote Procedure Call|Interprozess-Kommunikation|
|**TCP**|**4**|Transmission Control Protocol|Verbindungsorientierte, gesicherte Übertragung|
|**UDP**|**4**|User Datagram Protocol|Verbindungslos, schneller, aber ungesichert|
|**IP**|**3**|Internet Protocol|Paketvermittlung über IP-Adressen|

### Für die Prüfung besonders merken

**Schicht 7:** FTP, SMTP, HTTP, HTTPS  
**Schicht 5:** RPC  
**Schicht 4:** TCP, UDP  
**Schicht 3:** IP

Und der wichtigste Unterschied:

**TCP = zuverlässig/gesichert + verbindungsorientiert**  
**UDP = schneller + verbindungslos + keine gesicherte Übertragung**

Außerdem steht unten im Buch noch ein wichtiger Hinweis: Ein Begriff wie **FTP** kann sowohl das **Protokoll** als auch einen **Dienst bzw. eine Anwendung** (FTP-Server/FTP-Client) bezeichnen. Das erklärt auch deine frühere Frage, warum etwas gleichzeitig als Protokoll und Netzwerkdienst vorkommen kann.

**ICMP = Internet Control Message Protocol**

Es wird für **Kontroll- und Fehlermeldungen im IP-Netzwerk** verwendet.

Beispiel: **ping** verwendet ICMP, um zu prüfen, ob ein anderes Gerät erreichbar ist.

###### **DNS ist wie ein Telefonbuch fürs Internet.**

Du kennst den **Namen** einer Webseite, zum Beispiel:

google.com**

DNS sucht dazu die passende **IP-Adresse** heraus.

Also:

**Name → DNS → IP-Adresse**

Merksatz für die Prüfung: **DNS übersetzt Namen in IP-Adressen.** ✅



|IP-Bereich|Einsatzzweck|
|---|---|
|**192.168.0.1 – 192.168.0.50**|Client-Computer|
|**192.168.0.100 – 192.168.0.120**|Drucker|
|**192.168.0.140 – 192.168.0.160**|IP-Telefone|
|**192.168.0.200 – 192.168.0.230**|Verwaltbare Netzwerkgeräte (Switch, Kamera)|
|**192.168.0.250 – 192.168.0.254**|Server, Gateway (DSL-Router)|

![](Pasted%20image%2020261001182315.png)


![](Pasted%20image%2020261001195538.png)


0 bisch 099 netzwerkgeräte cam drucker nas 

und 200-254 offen laptops handys alles


---

## 🔗 Verknüpfungen zum Lernen

- [[Netzwerk Grunlagen|Netzwerk-Grundlagen]]
- [[Der weg zu Netzwerke|TCP/IP, Dienste & Protokolle]]
- [[IP submaske verstehen tabelle|IP-Adressierung & Subnetzmaske]]
- [[befehle und config 1|Befehle wie ping / ip / nmap]]
