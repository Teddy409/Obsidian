# Prüfungsvorbereitung Modul 117

**Thema:** Netzwerkgrundlagen  
**Dauer:** 105 Minuten  
**Maximalpunktzahl:** 100 Punkte

> [!important]
> Bearbeite zuerst alle Aufgaben. Öffne die Lösungen erst am Schluss.

## Zeitplan

| Teil | Thema | Zeit | Punkte |
|---|---|---:|---:|
| A | Netzwerk-Grundlagen | 10 Min. | 15 |
| B | Topologien | 15 Min. | 15 |
| C | OSI und TCP/IP | 20 Min. | 20 |
| D | Protokolle und Ports | 15 Min. | 15 |
| E | IPv4 und Subnetzmaske | 30 Min. | 25 |
| F | Praxis und Fehlersuche | 15 Min. | 10 |
| **Total** |  | **105 Min.** | **100** |

---

## Teil A – Netzwerk-Grundlagen (15 Punkte)

### Aufgabe 1 – Netzwerkarten (8 Punkte)

Erkläre **LAN**, **WLAN**, **MAN** und **WAN**. Nenne zu jedem Begriff ein Beispiel.

### Aufgabe 2 – Grundbegriffe (7 Punkte)

1. Was ist ein **SPOF**? Nenne ein Beispiel. (3 P.)
2. Was bedeutet **Redundanz**? Welchen Vorteil hat sie? (2 P.)
3. Was ist der Unterschied zwischen einer privaten und einer öffentlichen IP-Adresse? (2 P.)

---

## Teil B – Topologien (15 Punkte)

### Aufgabe 3 – Topologien vergleichen (9 Punkte)

Ergänze den Aufbau, einen Vorteil und einen Nachteil.

| Topologie | Aufbau | Vorteil | Nachteil |
|---|---|---|---|
| Stern |  |  |  |
| Bus |  |  |  |
| Ring |  |  |  |

### Aufgabe 4 – Firmennetzwerk (6 Punkte)

Eine kleine Firma besitzt acht Computer, zwei Drucker und einen Server.

1. Welche Topologie würdest du einsetzen? Begründe. (3 P.)
2. Welches Gerät ist normalerweise der zentrale Punkt? (1 P.)
3. Wie könnte man den wichtigsten SPOF reduzieren? (2 P.)

---

## Teil C – OSI und TCP/IP (20 Punkte)

### Aufgabe 5 – OSI-Schichten (7 Punkte)

Schreibe die sieben OSI-Schichten in der richtigen Reihenfolge auf. Beginne bei Schicht 1.

| Schicht | Name |
|---:|---|
| 1 |  |
| 2 |  |
| 3 |  |
| 4 |  |
| 5 |  |
| 6 |  |
| 7 |  |

### Aufgabe 6 – Begriffe zuordnen (8 Punkte)

Ordne jeden Begriff der richtigen OSI-Schicht zu.

| Begriff | OSI-Schicht |
|---|---:|
| Hub |  |
| Switch |  |
| MAC-Adresse |  |
| Router |  |
| IP |  |
| TCP |  |
| UDP |  |
| HTTP |  |

### Aufgabe 7 – TCP und UDP (5 Punkte)

Erkläre mindestens drei Unterschiede zwischen TCP und UDP. Nenne für beide je ein Anwendungsbeispiel.

---

## Teil D – Protokolle und Ports (15 Punkte)

### Aufgabe 8 – Tabelle ergänzen (10 Punkte)

| Protokoll | Aufgabe | Standard-Port |
|---|---|---:|
| HTTP |  |  |
| HTTPS |  |  |
| FTP-Steuerung |  |  |
| SMTP |  |  |
| POP3 |  |  |
| IMAP |  |  |
| DNS |  |  |

Für jede richtige Aufgabe gibt es 1 Punkt. Für HTTP, HTTPS und DNS gibt es zusätzlich je 1 Punkt für den richtigen Port.

### Aufgabe 9 – ARP, DNS und ICMP (5 Punkte)

1. Welche Aufgabe hat ARP? (2 P.)
2. Welche Aufgabe hat DNS? (2 P.)
3. Wofür wird ICMP beispielsweise verwendet? (1 P.)

---

## Teil E – IPv4 und Subnetzmaske (25 Punkte)

### Aufgabe 10 – IPv4-Grundlagen (5 Punkte)

1. Aus wie vielen Bits besteht eine IPv4-Adresse? (1 P.)
2. Wie viele Oktette besitzt sie? (1 P.)
3. Welchen Wertebereich kann ein Oktett haben? (1 P.)
4. Welche zwei Bestandteile bestimmt die Subnetzmaske? (2 P.)

### Aufgabe 11 – Privat oder öffentlich? (5 Punkte)

| IP-Adresse | Privat oder öffentlich? |
|---|---|
| `10.20.30.40` |  |
| `172.16.5.10` |  |
| `172.32.5.10` |  |
| `192.168.50.7` |  |
| `8.8.8.8` |  |

### Aufgabe 12 – Dezimal und Binär (6 Punkte)

1. Wandle `192` in eine 8-Bit-Binärzahl um. (2 P.)
2. Wandle `168` in eine 8-Bit-Binärzahl um. (2 P.)
3. Wandle `11111111` ins Dezimalsystem um. (1 P.)
4. Wandle `00000000` ins Dezimalsystem um. (1 P.)

### Aufgabe 13 – Subnetz `/24` (9 Punkte)

Gegeben:

- IP-Adresse: `192.168.10.37`
- Subnetzmaske: `255.255.255.0`
- Präfix: `/24`

1. Wie lautet die Netzwerkadresse? (2 P.)
2. Wie lautet die Broadcast-Adresse? (2 P.)
3. Welcher Hostbereich kann an Geräte vergeben werden? (2 P.)
4. Liegt `192.168.10.200` im gleichen Subnetz? Begründe. (2 P.)
5. Liegt `192.168.11.20` im gleichen Subnetz? (1 P.)

---

## Teil F – Praxis und Fehlersuche (10 Punkte)

### Aufgabe 14 – Netzwerkplan (6 Punkte)

Plane ein Netzwerk mit:

- Router `192.168.1.1`
- einem Switch
- zwei Computern
- einem Netzwerkdrucker
- einem WLAN-Laptop

Zeichne die Verbindungen. Vergib eindeutige IP-Adressen aus dem Netz `192.168.1.0/24`.

### Aufgabe 15 – Fehlersuche (4 Punkte)

Ein PC erreicht keine Webseite. Nenne für jeden Schritt einen passenden Linux-Befehl:

1. Eigene IP-Konfiguration anzeigen. (1 P.)
2. Erreichbarkeit des Routers testen. (1 P.)
3. Erreichbarkeit einer öffentlichen IP-Adresse testen. (1 P.)
4. Namensauflösung einer Domain testen. (1 P.)

---

# Lösungen

> [!success]- Lösungen Teil A
> **Aufgabe 1**
>
> - **LAN:** Lokales Netzwerk in einem kleinen Bereich, zum Beispiel in einer Schule.
> - **WLAN:** Kabelloses lokales Netzwerk, zum Beispiel ein Laptop am WLAN-Router.
> - **MAN:** Verbindet Netzwerke innerhalb einer Stadt oder Region.
> - **WAN:** Verbindet Netzwerke über grosse Entfernungen.
>
> **Aufgabe 2**
>
> 1. Ein SPOF ist eine einzelne Komponente, deren Ausfall das System unterbricht. Beispiel: der einzige Switch einer Stern-Topologie.
> 2. Bei Redundanz sind wichtige Komponenten oder Verbindungen mehrfach vorhanden. Beim Ausfall kann ein Ersatz übernehmen.
> 3. Private IP-Adressen werden im internen Netzwerk verwendet. Öffentliche IP-Adressen sind im Internet erreichbar.

> [!success]- Lösungen Teil B
> | Topologie | Aufbau | Vorteil | Nachteil |
> |---|---|---|---|
> | Stern | Alle Geräte sind mit einem Switch verbunden. | Ein Kabelausfall betrifft nur ein Gerät. | Der Switch ist ein SPOF. |
> | Bus | Alle Geräte teilen eine Hauptleitung. | Wenig Kabel. | Ausfall der Hauptleitung stört alle. |
> | Ring | Jedes Gerät ist mit zwei Nachbarn verbunden. | Geordneter Datenfluss. | Ein Unterbruch kann den Ring stören. |
>
> Für die Firma eignet sich eine Stern-Topologie. Sie ist gut erweiterbar und einfach zu warten. Der Switch ist der zentrale Punkt. Redundante Switches und unabhängige Ersatzverbindungen reduzieren den SPOF.

> [!success]- Lösungen Teil C
> **OSI-Schichten**
>
> 1. Bitübertragung / Physical
> 2. Sicherung / Data Link
> 3. Vermittlung / Network
> 4. Transport
> 5. Sitzung / Session
> 6. Darstellung / Presentation
> 7. Anwendung / Application
>
> **Zuordnung:** Hub 1, Switch 2, MAC-Adresse 2, Router 3, IP 3, TCP 4, UDP 4, HTTP 7.
>
> TCP ist verbindungsorientiert, bestätigt Daten und überträgt fehlende Daten erneut. Beispiel: HTTPS. UDP ist verbindungslos, bestätigt Pakete nicht und ist schneller. Beispiel: Live-Telefonie oder Streaming.

> [!success]- Lösungen Teil D
> | Protokoll | Aufgabe | Standard-Port |
> |---|---|---:|
> | HTTP | Unverschlüsselte Webseitenübertragung | 80/TCP |
> | HTTPS | Verschlüsselte Webseitenübertragung | 443/TCP |
> | FTP-Steuerung | Steuerung einer Dateiübertragung | 21/TCP |
> | SMTP | E-Mails versenden | 25/TCP |
> | POP3 | E-Mails abrufen | 110/TCP |
> | IMAP | E-Mails auf dem Server verwalten | 143/TCP |
> | DNS | Namen in IP-Adressen auflösen | 53/UDP und TCP |
>
> ARP ermittelt im lokalen IPv4-Netz die MAC-Adresse zu einer IP-Adresse. DNS übersetzt Domainnamen in IP-Adressen. ICMP dient Kontroll- und Fehlermeldungen; `ping` verwendet ICMP.

> [!success]- Lösungen Teil E
> **Aufgabe 10:** 32 Bits, 4 Oktette, Werte von 0 bis 255, Netzwerk- und Hostanteil.
>
> **Aufgabe 11:** privat, privat, öffentlich, privat, öffentlich.
>
> **Aufgabe 12:** `11000000`, `10101000`, `255`, `0`.
>
> **Aufgabe 13**
>
> 1. Netzwerkadresse: `192.168.10.0`
> 2. Broadcast-Adresse: `192.168.10.255`
> 3. Hostbereich: `192.168.10.1` bis `192.168.10.254`
> 4. Ja, die ersten drei Oktette stimmen bei `/24` überein.
> 5. Nein.

> [!success]- Lösungen Teil F
> **Beispiel-Netzwerkplan**
>
> ```text
> Internet
>    |
> Router 192.168.1.1
>    |
> Switch
>    |-- PC 1:    192.168.1.20
>    |-- PC 2:    192.168.1.21
>    |-- Drucker: 192.168.1.50
>    `-- WLAN-Laptop über Router: 192.168.1.30
> ```
>
> **Befehle**
>
> 1. `ip address`
> 2. `ping -c 3 192.168.1.1`
> 3. `ping -c 3 8.8.8.8`
> 4. `nslookup example.com` oder `dig example.com`

---

## Auswertung

| Punkte | Einschätzung |
|---:|---|
| 90–100 | Sehr gut vorbereitet |
| 80–89 | Gut vorbereitet |
| 70–79 | Solide, einzelne Themen wiederholen |
| 60–69 | Grundlagen vorhanden, gezielt nacharbeiten |
| unter 60 | Lernstoff nochmals durcharbeiten |
