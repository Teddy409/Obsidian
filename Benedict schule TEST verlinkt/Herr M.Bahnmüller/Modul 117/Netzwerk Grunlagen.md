
# Kapitel 1 Netzwerkbau/ dienst

### Netzwerkbau/ dienst

```
Fachbegriffe in diesem Block

Netzwerktopolgien,SPOF,Backbone,Glasfasser, Eterneth, MAC-Adresse, Abschrimung, Subnet-Maske,Private IP-Adressen , IPv4, IPv6 OSI Refernezmodelle, usw.

SPOF = Single , Poin OF FAilure

Das ist **eine einzelne Stelle, deren Ausfall das ganze System stoppen kann**.

Beispiel: Bei einer **Stern-Topologie** ist der zentrale **Switch** ein SPOF. Fällt der Switch aus, können die angeschlossenen Geräte nicht mehr miteinander kommunizieren.
```

````
```Redundanz = etwas ist doppelt vorhanden, damit bei einem Ausfall trotzdem alles weiterläuft.
Beispiel:  
Du hast **zwei Switches** statt nur einen.

Fällt **Switch 1** aus, kann **Switch 2** übernehmen.

Damit verhindert man einen **SPOF**.

Kurz:  
**SPOF = eine kritische Stelle**  
**Redundanz = Ersatz vorhanden**


Beispiel: Dein Laptop ist per **LAN-Kabel** verbunden und zusätzlich mit **WLAN**. Fällt das LAN aus und der Laptop wechselt auf WLAN, hast du eine Ersatzverbindung.

Aber nur dann ist es echte Redundanz, wenn **nicht beide am gleichen SPOF hängen**. Wenn LAN und WLAN am gleichen Router hängen und der Router ausfällt, bringen dir beide Verbindungen nichts.

````

# Netzwerkarchitektur

90% ist stern am meist verbaut

Topologien

Aufgaben: 

lerne WAN GAN WLAN 

[[Pasted image 20260903212000.png]]

[[Pasted image 20260903212404.png]]


**WLAN ist nur die Funk-Verbindung zwischen deinem Gerät und dem Router.**  
**Internet ist die Verbindung vom Router nach draussen ins weltweite Netz.**

Beispiel:

**Laptop → WLAN → Router → Internet**

Wenn das Internet ausfällt, bleibt dieser Teil trotzdem bestehen:

**Laptop → WLAN → Router**

Darum kann **WLAN funktionieren, obwohl Internet nicht funktioniert**.

Für die Schule reicht:

**WLAN = kabelloses lokales Netzwerk. Internet = weltweite Verbindung vieler Netzwerke.**





- **LAN/WLAN** = dein lokales Netzwerk
- **WAN** = verbindet Netzwerke über grössere Entfernungen
- **GAN** = Netzwerk über weltweite Entfernungen
- **Internet** = das riesige weltweite Netz aus sehr vielen einzelnen Netzwerken

Der wichtigste Satz ist:

**Internet = viele Netzwerke, die miteinander verbunden sind.**

Also: **Alles im Internet ist Netzwerk, aber nicht jedes Netzwerk ist Internet.**


## **Netzwerktechnik**

eigenschaften LAN / WLAN


 ## Private und öffentliche IP-Adressen

### Private IP-Adresse

Eine **private IP-Adresse** wird **innerhalb eines privaten Netzwerks (LAN)** verwendet.

Beispiel zuhause:

**PC → Switch/WLAN → Router**

Dein PC könnte z. B. diese Adresse haben:

**192.168.1.20**

Diese Adresse funktioniert innerhalb deines Netzwerks, wird aber **nicht direkt im öffentlichen Internet verwendet**.

Private IPv4-Bereiche aus deinem Lernstoff:

|Privater Bereich|
|---|
|**10.0.0.0 – 10.255.255.255**|
|**172.16.0.0 – 172.31.255.255**|
|**192.168.0.0 – 192.168.255.255**|

### Öffentliche IP-Adresse

Eine **öffentliche IP-Adresse** wird für die Kommunikation **im Internet** verwendet.

Wenn dein privater PC ins Internet möchte, läuft die Verbindung normalerweise über deinen **Router**:

**PC mit privater IP → Router → öffentliche IP → Internet**

Der Router setzt dabei typischerweise private Adressen auf seine öffentliche Adresse um (**NAT/PAT**).

### Einfach merken

**Privat = innerhalb des eigenen Netzwerks** 🏠  
**Öffentlich = im Internet** 🌍

Beispiel:

**192.168.1.20** → privat  
**Router** → Übergang  
**öffentliche IP** → Internet

---

## 🔗 Verknüpfungen zum Lernen

- [[Der weg zu Netzwerke|Entstehung & Arten von Netzwerken]]
- [[Topoligie Netzwerke|Netzwerk-Topologien]]
- [[OSI Modelle|OSI-Modell & Protokolle]]
- [[IP submaske verstehen tabelle|IPv4 & Subnetzmaske]]
- [[Dezimal Bit|Dezimal / Bit-Grundlagen]]
- [[befehle und config 1|Netzwerk-Befehle & Konfiguration]]
- [[aufgabe|Praxisaufgabe Netzwerkplan]]
