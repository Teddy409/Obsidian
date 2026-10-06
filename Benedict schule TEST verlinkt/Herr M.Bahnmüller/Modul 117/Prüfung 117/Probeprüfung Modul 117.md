# Probeprüfung Modul 117 – Netzwerke

**Bearbeitungszeit:** 120 Minuten  
**Punkte:** 120  
**Hilfsmittel:** Schreibzeug und Taschenrechner

> [!important]
> Öffne die eingeklappten Lösungen erst, nachdem du alle Aufgaben bearbeitet hast.

## Zeitplan

| Teil | Thema | Zeit | Punkte |
|---|---|---:|---:|
| A | Netzwerk-Grundlagen | 10 Min. | 15 |
| B | Topologien | 20 Min. | 20 |
| C | OSI und TCP/IP | 25 Min. | 25 |
| D | Protokolle und Ports | 15 Min. | 15 |
| E | IPv4 und Subnetzmaske | 35 Min. | 31 |
| F | Praxis und Fehlersuche | 15 Min. | 14 |
| **Total** |  | **120 Min.** | **120** |

---

## Teil A – Netzwerk-Grundlagen (15 Punkte)

### Aufgabe 1 – Netzwerkarten (8 Punkte)

Erkläre **LAN**, **WLAN**, **MAN** und **WAN**. Nenne zu jedem Begriff ein Beispiel.

### Aufgabe 2 – Grundbegriffe (7 Punkte)

1. Was ist ein **SPOF**? Nenne ein Beispiel. (3 P.)
2. Was bedeutet **Redundanz** und welchen Vorteil hat sie? (2 P.)
3. Erkläre den Unterschied zwischen einer privaten und einer öffentlichen IP-Adresse. (2 P.)

---

## Teil B – Topologien (20 Punkte)

### Aufgabe 3 – Alle Topologien im Vergleich (14 Punkte)

Ergänze zu jeder Topologie den Aufbau, einen Vorteil und einen Nachteil. (je 2 P.)

| Topologie | Aufbau | Vorteil | Nachteil |
|---|---|---|---|
| Stern |  |  |  |
| Bus |  |  |  |
| Ring |  |  |  |
| Linie |  |  |  |
| Baum |  |  |  |
| Teilvermascht |  |  |  |
| Vollvermascht |  |  |  |

### Aufgabe 4 – Firmennetzwerk (6 Punkte)

Eine Firma besitzt acht Computer, zwei Drucker und einen Server.

1. Welche Topologie würdest du verwenden? Begründe. (3 P.)
2. Welches Gerät ist normalerweise der zentrale Punkt? (1 P.)
3. Wie könnte man den wichtigsten SPOF reduzieren? (2 P.)

---

## Teil C – OSI und TCP/IP (25 Punkte)

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

Ordne jeden Begriff der richtigen OSI-Schicht zu:

**Switch, Router, Hub, IP, MAC-Adresse, TCP, UDP, HTTP**

| Begriff | OSI-Schicht |
|---|---:|
| Switch |  |
| Router |  |
| Hub |  |
| IP |  |
| MAC-Adresse |  |
| TCP |  |
| UDP |  |
| HTTP |  |

### Aufgabe 7 – TCP und UDP (5 Punkte)

Erkläre mindestens drei Unterschiede zwischen TCP und UDP. Nenne für beide je ein Anwendungsbeispiel.

### Aufgabe 8 – OSI-Komponenten zuordnen (5 Punkte)

Ordne jede Komponente der Schicht zu, auf der sie laut Lernunterlage arbeitet (je 1 P.):

**Hub, Switch, Router, Stateful-Inspection-Firewall, Proxy**

| Komponente | OSI-Schicht |
|---|---:|
| Hub |  |
| Switch |  |
| Router |  |
| Stateful-Inspection-Firewall |  |
| Proxy |  |

---

## Teil D – Protokolle und Ports (15 Punkte)

### Aufgabe 9 – Protokolltabelle (10 Punkte)

Ergänze Aufgabe und Standard-Port.

| Protokoll | Aufgabe | Port |
|---|---|---:|
| HTTP |  |  |
| HTTPS |  |  |
| FTP-Steuerung |  |  |
| SMTP |  |  |
| POP3 |  |  |
| IMAP |  |  |
| DNS |  |  |

Für jede richtige Aufgabe gibt es 1 Punkt. Für HTTP, HTTPS und DNS gibt es zusätzlich je 1 Punkt für den richtigen Port.

### Aufgabe 10 – ARP, DNS und ICMP (5 Punkte)

1. Welche Aufgabe hat ARP? (2 P.)
2. Welche Aufgabe hat DNS? (2 P.)
3. Wofür wird ICMP beispielsweise verwendet? (1 P.)

---

## Teil E – IPv4 und Subnetzmaske (31 Punkte)

### Aufgabe 11 – IPv4-Grundlagen (5 Punkte)

1. Aus wie vielen Bits besteht eine IPv4-Adresse? (1 P.)
2. Wie viele Oktette besitzt sie? (1 P.)
3. Welchen Wertebereich kann ein Oktett haben? (1 P.)
4. Welche zwei Bestandteile bestimmt die Subnetzmaske? (2 P.)

### Aufgabe 12 – Privat oder öffentlich? (5 Punkte)

| IP-Adresse | Privat oder öffentlich? |
|---|---|
| `10.20.30.40` |  |
| `172.16.5.10` |  |
| `172.32.5.10` |  |
| `192.168.50.7` |  |
| `8.8.8.8` |  |

### Aufgabe 13 – Dezimal und Binär (6 Punkte)

1. Wandle `192` in eine 8-Bit-Binärzahl um. (2 P.)
2. Wandle `168` in eine 8-Bit-Binärzahl um. (2 P.)
3. Wandle `11111111` ins Dezimalsystem um. (1 P.)
4. Wandle `00000000` ins Dezimalsystem um. (1 P.)

### Aufgabe 14 – Subnetz `/24` (9 Punkte)

Gegeben:

- IP-Adresse: `192.168.10.37`
- Subnetzmaske: `255.255.255.0`
- Präfix: `/24`

1. Wie lautet die Netzwerkadresse? (2 P.)
2. Wie lautet die Broadcast-Adresse? (2 P.)
3. Welcher Hostbereich kann an Geräte vergeben werden? (2 P.)
4. Liegt `192.168.10.200` im gleichen Subnetz? Begründe. (2 P.)
5. Liegt `192.168.11.20` im gleichen Subnetz? (1 P.)

### Aufgabe 15 – Subnetz-Berechnung `/27` (6 Punkte)

Gegeben:

- IP-Adresse: `192.168.20.75`
- Präfix: `/27`

1. Wie lautet die Subnetzmaske in Dezimalschreibweise? (1 P.)
2. Wie lautet die Netzwerkadresse? (2 P.)
3. Wie lautet die Broadcast-Adresse? (1 P.)
4. Wie viele nutzbare Host-Adressen gibt es in diesem Subnetz? (2 P.)

---

## Teil F – Praxis und Fehlersuche (14 Punkte)

### Aufgabe 16 – Netzwerkplan mit IP-Zuteilungsschema (9 Punkte)

Eine Firma nutzt im Netz `192.168.0.0/24` folgendes Zuteilungsschema:

| IP-Bereich | Einsatzzweck |
|---|---|
| `192.168.0.1 – 192.168.0.50` | Client-Computer |
| `192.168.0.100 – 192.168.0.120` | Drucker |
| `192.168.0.140 – 192.168.0.160` | IP-Telefone |
| `192.168.0.200 – 192.168.0.230` | Verwaltbare Netzwerkgeräte (Switch) |
| `192.168.0.250 – 192.168.0.254` | Server, Gateway (Router) |

Plane ein Netzwerk mit: einem Router/Gateway, einem verwaltbaren Switch, drei PCs, einem Netzwerkdrucker und einem IP-Telefon.

1. Zeichne den Netzwerkplan mit allen Verbindungen. (3 P.)
2. Vergib für jedes Gerät eine passende IP-Adresse gemäss obigem Schema. (4 P.)
3. Begründe kurz, warum ein solches Zuteilungsschema in der Praxis sinnvoll ist. (2 P.)

### Aufgabe 17 – Fehlersuche (5 Punkte)

Ein PC erreicht keine Webseite. Nenne für jeden Schritt einen passenden Linux-Befehl:

1. Eigene IP-Konfiguration anzeigen. (1 P.)
2. Erreichbarkeit des Routers testen. (1 P.)
3. Erreichbarkeit einer öffentlichen IP-Adresse testen. (1 P.)
4. Namensauflösung einer Domain testen. (1 P.)
5. Den Weg der Pakete bis zum Ziel anzeigen. (1 P.)

---

# Lösungen

> [!success]- Lösungen Teil A
> **Aufgabe 1**
>
> - **LAN:** Lokales Netzwerk in einem begrenzten Bereich, etwa in einer Schule.
> - **WLAN:** Kabelloses lokales Netzwerk, etwa ein Laptop am WLAN-Router.
> - **MAN:** Verbindet Netzwerke innerhalb einer Stadt oder Region.
> - **WAN:** Verbindet Netzwerke über grosse Entfernungen.
>
> **Aufgabe 2**
>
> 1. Ein SPOF ist eine einzelne Komponente, deren Ausfall das System unterbricht. Beispiel: der einzige Switch einer Stern-Topologie.
> 2. Bei Redundanz sind wichtige Komponenten oder Wege mehrfach vorhanden. Bei einem Ausfall kann ein Ersatz übernehmen.
> 3. Private Adressen werden intern verwendet und nicht direkt im Internet geroutet. Öffentliche Adressen sind im Internet eindeutig erreichbar.

> [!success]- Lösungen Teil B
> **Aufgabe 3**
>
> | Topologie | Aufbau | Vorteil | Nachteil |
> |---|---|---|---|
> | Stern | Alle Geräte sind mit einem zentralen Switch/Router verbunden. | Ein Kabelausfall betrifft nur ein Gerät. | Der zentrale Switch ist ein SPOF. |
> | Bus | Alle Geräte teilen sich eine gemeinsame Hauptleitung. | Wenig Kabel, einfacher Aufbau. | Ausfall der Hauptleitung stört alle Geräte. |
> | Ring | Jedes Gerät ist mit zwei Nachbarn verbunden, es entsteht ein Kreis. | Geordneter Datenfluss. | Ein Unterbruch kann den ganzen Ring stören. |
> | Linie | Geräte sind hintereinander wie eine Kette verbunden. | Einfach und wenig Verkabelung. | Ein Unterbruch trennt nachfolgende Geräte. |
> | Baum | Mehrere kleinere Netzwerke (Sterne) sind wie Äste an einem Hauptknoten verbunden. | Gut erweiterbar und übersichtlich. | Fällt ein Hauptknoten aus, sind viele Geräte betroffen. |
> | Teilvermascht | Einige Geräte sind direkt mit mehreren anderen verbunden, aber nicht alle untereinander. | Mehrere mögliche Datenwege, ausfallsicherer. | Mehr Kabel und aufwendigerer Aufbau. |
> | Vollvermascht | Jedes Gerät ist direkt mit jedem anderen Gerät verbunden. | Sehr hohe Ausfallsicherheit. | Sehr viele Verbindungen, teuer und kompliziert. |
>
> **Aufgabe 4**
>
> 1. Stern-Topologie: gut erweiterbar und einfach zu warten.
> 2. Ein Switch.
> 3. Redundante Switches und unabhängige Ersatzverbindungen.

> [!success]- Lösungen Teil C
> **Aufgabe 5**
>
> 1. Bitübertragung / Physical
> 2. Sicherung / Data Link
> 3. Vermittlung / Network
> 4. Transport
> 5. Sitzung / Session
> 6. Darstellung / Presentation
> 7. Anwendung / Application
>
> **Aufgabe 6**
>
> | Begriff | Schicht |
> |---|---:|
> | Switch | 2 |
> | Router | 3 |
> | Hub | 1 |
> | IP | 3 |
> | MAC-Adresse | 2 |
> | TCP | 4 |
> | UDP | 4 |
> | HTTP | 7 |
>
> **Aufgabe 7**
>
> TCP ist verbindungsorientiert, bestätigt Daten und überträgt fehlende Daten erneut. Es ist zuverlässig, aber aufwendiger. Beispiel: HTTPS.
>
> UDP ist verbindungslos, bestätigt Pakete nicht und ist schneller. Beispiel: Live-Telefonie oder Streaming.
>
> **Aufgabe 8**
>
> | Komponente | Schicht |
> |---|---:|
> | Hub | 1 |
> | Switch | 2 |
> | Router | 3 |
> | Stateful-Inspection-Firewall | 4 |
> | Proxy | 7 |

> [!success]- Lösungen Teil D
> **Aufgabe 9**
>
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
> **Aufgabe 10**
>
> 1. ARP ermittelt im lokalen IPv4-Netz die MAC-Adresse zu einer IP-Adresse.
> 2. DNS übersetzt Domainnamen in IP-Adressen.
> 3. ICMP dient Kontroll- und Fehlermeldungen. `ping` verwendet ICMP.

> [!success]- Lösungen Teil E
> **Aufgabe 11:** 32 Bits; 4 Oktette; Werte von 0 bis 255; Netzwerk- und Hostanteil.
>
> **Aufgabe 12**
>
> - `10.20.30.40`: privat
> - `172.16.5.10`: privat
> - `172.32.5.10`: öffentlich
> - `192.168.50.7`: privat
> - `8.8.8.8`: öffentlich
>
> **Aufgabe 13**
>
> 1. `192` = `11000000`
> 2. `168` = `10101000`
> 3. `11111111` = `255`
> 4. `00000000` = `0`
>
> **Aufgabe 14**
>
> 1. Netzwerkadresse: `192.168.10.0`
> 2. Broadcast-Adresse: `192.168.10.255`
> 3. Hostbereich: `192.168.10.1` bis `192.168.10.254`
> 4. Ja, die ersten drei Oktette stimmen bei `/24` überein.
> 5. Nein.
>
> **Aufgabe 15**
>
> 1. Subnetzmaske: `255.255.255.224`
> 2. Netzwerkadresse: `192.168.20.64` (Blockgrösse 32, `75` liegt im Block `64–95`)
> 3. Broadcast-Adresse: `192.168.20.95`
> 4. Nutzbare Hosts: `2^5 − 2 = 30` (Hostbereich `192.168.20.65 – 192.168.20.94`)

> [!success]- Lösungen Teil F
> **Aufgabe 16 – Beispiel**
>
> ```text
> Internet
>    |
> Router/Gateway: 192.168.0.250
>    |
> Switch (verwaltbar): 192.168.0.200
>    |-- PC 1:      192.168.0.10
>    |-- PC 2:      192.168.0.11
>    |-- PC 3:      192.168.0.12
>    |-- Drucker:   192.168.0.100
>    `-- IP-Telefon: 192.168.0.140
> ```
>
> Ein solches Schema ist sinnvoll, weil man anhand der IP-Adresse sofort erkennt, um welche Geräteart es sich handelt. Das erleichtert Fehlersuche, Firewall-Regeln und die Verwaltung grösserer Netzwerke.
>
> **Aufgabe 17**
>
> 1. `ip address`
> 2. `ping -c 3 192.168.1.1`
> 3. `ping -c 3 8.8.8.8`
> 4. `nslookup example.com` oder `dig example.com`
> 5. `traceroute example.com` (oder `tracepath example.com`)

---

## Auswertung

| Punkte | Einschätzung |
|---:|---|
| 108–120 | Sehr gut vorbereitet |
| 96–107 | Gut vorbereitet |
| 84–95 | Solide, einzelne Themen wiederholen |
| 72–83 | Grundlagen vorhanden, gezielt nacharbeiten |
| unter 72 | Lernstoff nochmals durcharbeiten |
