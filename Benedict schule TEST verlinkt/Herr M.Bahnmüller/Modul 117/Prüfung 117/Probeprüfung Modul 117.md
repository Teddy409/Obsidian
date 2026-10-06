# Probeprüfung Modul 117 – Block 1 bis 4

**Thema:** Informatik- und Netzinfrastruktur für ein kleines Unternehmen realisieren  
**Bearbeitungszeit:** 120 Minuten  
**Maximalpunktzahl:** 120 Punkte  
**Hilfsmittel:** eigene Zusammenfassung, Unterrichtsunterlagen und Taschenrechner

> [!important]
> Bearbeite die Prüfung zuerst vollständig auf Papier. Öffne die Musterlösungen erst nach Ablauf der 120 Minuten.

## Zeit- und Punkteplan

| Teil | Thema | Richtzeit | Punkte |
|---|---|---:|---:|
| A | Netzwerkarchitektur und Topologien | 10 Min. | 12 |
| B | Medien und Komponenten | 15 Min. | 16 |
| C | OSI, TCP/IP und Protokolle | 20 Min. | 20 |
| D | Adressierung und Subnetting | 25 Min. | 24 |
| E | Projektvorgehen | 15 Min. | 14 |
| F | Praktisches Netzkonzept | 25 Min. | 24 |
| G | Inbetriebnahme und Fehlersuche | 10 Min. | 10 |
| **Total** |  | **120 Min.** | **120** |

---

# Prüfung

## Teil A – Netzwerkarchitektur und Topologien (12 Punkte)

### Aufgabe 1 – Netzwerkarten (5 Punkte)

Erkläre die folgenden Begriffe jeweils in einem Satz und nenne für vier davon ein passendes Beispiel:

1. LAN
2. WLAN
3. MAN
4. WAN
5. GAN

### Aufgabe 2 – Topologie, SPOF und Redundanz (7 Punkte)

Eine kleine Firma hat zwölf Arbeitsplätze, zwei Drucker, ein NAS und einen Internetrouter.

1. Welche Topologie würdest du einsetzen? Begründe mit zwei Vorteilen. (3 P.)
2. Nenne den wichtigsten SPOF dieser Topologie. (1 P.)
3. Schlage zwei konkrete Massnahmen vor, die die Ausfallsicherheit erhöhen. (2 P.)
4. Was ist ein Backbone? (1 P.)

---

## Teil B – Medien und Komponenten (16 Punkte)

### Aufgabe 3 – Übertragungsmedien auswählen (8 Punkte)

Wähle jeweils **Twisted Pair**, **Glasfaser** oder **WLAN** und begründe deine Wahl.

1. Ein Büro-PC steht fünf Meter vom Switch entfernt. (2 P.)
2. Zwei Gebäude liegen 400 Meter auseinander; zwischen ihnen treten starke elektromagnetische Störungen auf. (2 P.)
3. Mitarbeitende sollen sich mit Tablets frei im Sitzungszimmer bewegen. (2 P.)
4. Erkläre den Unterschied zwischen ungeschirmtem und geschirmtem Twisted-Pair-Kabel. (2 P.)

### Aufgabe 4 – Komponenten zuordnen (8 Punkte)

Ergänze Hauptaufgabe und typische OSI-Schicht.

| Komponente | Hauptaufgabe | OSI-Schicht |
|---|---|---:|
| Hub |  |  |
| Switch |  |  |
| Router |  |  |
| Access Point |  |  |
| Medienkonverter |  |  |
| Stateful Firewall |  |  |
| Proxy |  |  |
| SFP-Modul |  |  |

Pro Zeile gibt es 0,5 Punkte für die Aufgabe und 0,5 Punkte für die Schicht.

---

## Teil C – OSI, TCP/IP und Protokolle (20 Punkte)

### Aufgabe 5 – OSI-Modell (7 Punkte)

Schreibe die sieben OSI-Schichten von Schicht 1 bis 7 auf. Deutsch oder Englisch genügt.

| Schicht | Name |
|---:|---|
| 1 |  |
| 2 |  |
| 3 |  |
| 4 |  |
| 5 |  |
| 6 |  |
| 7 |  |

### Aufgabe 6 – Begriffe und Protokolle (8 Punkte)

Ergänze Aufgabe und OSI-Schicht.

| Begriff | Aufgabe | OSI-Schicht |
|---|---|---:|
| MAC-Adresse |  |  |
| ARP |  |  |
| IP |  |  |
| ICMP |  |  |
| TCP |  |  |
| UDP |  |  |
| DNS |  |  |
| HTTPS |  |  |

Pro Zeile gibt es 0,5 Punkte für die Aufgabe und 0,5 Punkte für die Schicht.

### Aufgabe 7 – TCP und UDP (5 Punkte)

1. Nenne drei Unterschiede zwischen TCP und UDP. (3 P.)
2. Nenne je ein sinnvolles Anwendungsbeispiel. (2 P.)

---

## Teil D – Adressierung und Subnetting (24 Punkte)

### Aufgabe 8 – IPv4-Grundlagen (5 Punkte)

1. Aus wie vielen Bits und Oktetten besteht IPv4? (2 P.)
2. Welchen Wertebereich hat ein Oktett? (1 P.)
3. Was trennt die Subnetzmaske? (1 P.)
4. Wozu dient das Default Gateway? (1 P.)

### Aufgabe 9 – Private Adressen (4 Punkte)

Markiere jede Adresse als **privat** oder **öffentlich**.

| Adresse | privat / öffentlich |
|---|---|
| `10.25.8.4` |  |
| `172.20.100.5` |  |
| `172.32.1.5` |  |
| `192.168.80.20` |  |

### Aufgabe 10 – Binär und Maske (4 Punkte)

1. Wandle `192` in eine 8-Bit-Binärzahl um. (1 P.)
2. Wandle `224` in eine 8-Bit-Binärzahl um. (1 P.)
3. Welche Dezimalmaske gehört zu `/27`? (1 P.)
4. Wie viele Hostbits bleiben bei `/27`? (1 P.)

### Aufgabe 11 – Subnetz vollständig berechnen (9 Punkte)

Gegeben ist die Hostadresse `192.168.40.78/27`.

1. Subnetzmaske in Dezimalschreibweise (1 P.)
2. Blockgrösse im letzten Oktett (1 P.)
3. Netzwerkadresse (2 P.)
4. Broadcast-Adresse (2 P.)
5. erster und letzter nutzbarer Host (2 P.)
6. Anzahl nutzbarer Hosts (1 P.)

### Aufgabe 12 – MAC und IPv6 (2 Punkte)

1. Wie lang ist eine klassische MAC-Adresse und wofür wird sie verwendet? (1 P.)
2. Wie lang ist eine IPv6-Adresse und warum wurde IPv6 eingeführt? (1 P.)

---

## Teil E – Projektvorgehen (14 Punkte)

### Aufgabe 13 – Projekt-Vorphase (8 Punkte)

Eine Bäckerei eröffnet eine zweite Filiale. Dort werden sechs PCs, zwei Kassensysteme, ein Netzwerkdrucker, WLAN für Mitarbeitende und ein zentraler Dateispeicher benötigt.

1. Nenne vier Informationen, die du für das Firmenporträt und die Ausgangslage erheben musst. (2 P.)
2. Erkläre den Unterschied zwischen IST- und SOLL-Zustand mit je einem Beispiel aus diesem Projekt. (2 P.)
3. Formuliere zwei überprüfbare Projektziele. (2 P.)
4. Warum müssen Budget und Termin schon in der Vorphase bekannt sein? (2 P.)

### Aufgabe 14 – Phasen und Ergebnisse (6 Punkte)

Ordne jedem Ergebnis eine sinnvolle Projektphase zu:

| Ergebnis | Projektphase |
|---|---|
| Anforderungen und IST-Aufnahme |  |
| Variantenvergleich und Netzkonzept |  |
| Termin-, Budget- und Materialplan |  |
| montierte und konfigurierte Geräte |  |
| Testprotokoll und Abnahme |  |
| Betriebsanleitung und Übergabe |  |

---

## Teil F – Praktisches Netzkonzept (24 Punkte)

### Ausgangslage

Die Bäckerei aus Teil E erhält das Netz `192.168.50.0/24`.

Benötigt werden:

- ein Router/Firewall mit Internetanschluss
- ein verwaltbarer Switch
- ein Access Point
- sechs Büro-PCs
- zwei Kassensysteme
- ein Netzwerkdrucker
- ein NAS

Das Unternehmen legt folgende Bereiche fest:

| Bereich | Verwendung |
|---|---|
| `.1 – .19` | Router, Switch und Access Point |
| `.20 – .39` | Server, NAS und Management |
| `.40 – .59` | Drucker und Spezialgeräte |
| `.100 – .199` | DHCP-Clients |
| `.200 – .219` | Kassensysteme mit statischer IP |

### Aufgabe 15 – Netzwerkplan zeichnen (6 Punkte)

Zeichne einen vollständigen Netzplan. Er muss enthalten:

- Internet, Router/Firewall, Switch und Access Point
- NAS, Drucker, sechs PCs und zwei Kassensysteme
- alle Kabel- und WLAN-Verbindungen
- Gerätenamen sowie IP-Adressen oder Adressierungsart

### Aufgabe 16 – IP-Plan (8 Punkte)

Ergänze einen gültigen IP-Plan. Verwende keine Adresse doppelt.

| Gerät | IP-Adresse | Maske/Präfix | Gateway | statisch/DHCP |
|---|---|---|---|---|
| Router R01 |  |  |  |  |
| Switch SW01 |  |  |  |  |
| Access Point AP01 |  |  |  |  |
| NAS01 |  |  |  |  |
| Drucker PRN01 |  |  |  |  |
| Kasse POS01 |  |  |  |  |
| Kasse POS02 |  |  |  |  |
| Büro-PCs |  |  |  |  |

### Aufgabe 17 – Material und Budget (6 Punkte)

1. Nenne sechs notwendige Positionen für die Materialliste. Mengen müssen sinnvoll sein. (3 P.)
2. Welche fünf Angaben gehören pro gekaufter Hardwareposition in den Budgetplan? (2 P.)
3. Nenne ein technisches Auswahlkriterium für den Switch. (1 P.)

### Aufgabe 18 – Dokumentation (4 Punkte)

Nenne je vier Inhalte:

1. eines guten Netzplans (2 P.)
2. eines Konfigurations- oder Betriebshandbuchs für den Router (2 P.)

---

## Teil G – Inbetriebnahme und Fehlersuche (10 Punkte)

### Aufgabe 19 – Kein Internetzugang (10 Punkte)

Ein Büro-PC kann keine Webseite öffnen. Nenne zu jedem Schritt eine passende Kontrolle oder einen Linux-Befehl und beschreibe kurz, was damit geprüft wird.

1. Physische Verbindung (1 P.)
2. Eigene IP-Konfiguration (2 P.)
3. Verbindung zum Default Gateway (2 P.)
4. Verbindung ins Internet ohne DNS (2 P.)
5. Namensauflösung (2 P.)
6. Weg der Pakete (1 P.)

---

# Musterlösungen

> [!success]- Teil A – Netzwerkarchitektur und Topologien
> **Aufgabe 1**
>
> - **LAN:** Lokales Netz in einem begrenzten Bereich, zum Beispiel ein Büronetz.
> - **WLAN:** Drahtloses LAN, zum Beispiel Tablets über einen Access Point.
> - **MAN:** Verbindet Netze innerhalb einer Stadt oder Region.
> - **WAN:** Verbindet Netze über grosse Entfernungen, zum Beispiel zwei Firmensitze.
> - **GAN:** Weltweite Verbindung von Netzen, zum Beispiel ein globales Unternehmensnetz.
>
> **Aufgabe 2**
>
> 1. Stern- oder Baumtopologie. Sie ist gut erweiterbar und ein defektes Endgerätekabel stört die anderen Geräte nicht.
> 2. Der zentrale Switch, je nach Aufbau auch Router oder Stromversorgung.
> 3. Zum Beispiel zweiter Switch mit unabhängigen Uplinks, redundanter Router/Internetanschluss, USV oder redundante Stromversorgung. Die Ersatzwege dürfen nicht am gleichen SPOF hängen.
> 4. Ein Backbone ist die leistungsfähige Hauptverbindung zwischen Netzbereichen.

> [!success]- Teil B – Medien und Komponenten
> **Aufgabe 3**
>
> 1. Twisted Pair: kurze, feste und günstige Büroverbindung.
> 2. Glasfaser: grosse Distanz und unempfindlich gegen elektromagnetische Störungen.
> 3. WLAN: ermöglicht Mobilität ohne Kabel zum Endgerät.
> 4. UTP hat keine zusätzliche Schirmung. STP/FTP besitzt Folien- oder Geflechtschirmung und schützt besser gegen elektromagnetische Störungen, muss aber fachgerecht installiert werden.
>
> **Aufgabe 4**
>
> | Komponente | Hauptaufgabe | OSI |
> |---|---|---:|
> | Hub | Bits an alle Ports verteilen | 1 |
> | Switch | Frames anhand MAC-Adressen weiterleiten | 2 |
> | Router | Pakete zwischen IP-Netzen routen | 3 |
> | Access Point | WLAN mit kabelgebundenem LAN verbinden | 2 |
> | Medienkonverter | physisches Medium/Signal umwandeln | 1 |
> | Stateful Firewall | Verbindungen und Ports zustandsbezogen filtern | 4 |
> | Proxy | Anwendungsanfragen vermitteln | 7 |
> | SFP-Modul | elektrisches/optisches Senden und Empfangen | 1 |

> [!success]- Teil C – OSI, TCP/IP und Protokolle
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
> | Begriff | Aufgabe | OSI |
> |---|---|---:|
> | MAC-Adresse | lokale physikalische Adressierung | 2 |
> | ARP | IPv4-Adresse lokal in MAC-Adresse auflösen | 2/3 |
> | IP | logische Adressierung und Paketvermittlung | 3 |
> | ICMP | Kontroll- und Fehlermeldungen | 3 |
> | TCP | zuverlässiger, verbindungsorientierter Transport | 4 |
> | UDP | schneller, verbindungsloser Transport | 4 |
> | DNS | Namen und IP-Adressen auflösen | 7 |
> | HTTPS | verschlüsselte Webseitenübertragung | 7 |
>
> **Aufgabe 7**
>
> TCP baut eine Verbindung auf, bestätigt Daten, hält die Reihenfolge ein und überträgt Verluste erneut. UDP sendet ohne Verbindungsaufbau, Bestätigung oder Zustellgarantie und hat weniger Overhead. TCP-Beispiel: HTTPS oder Dateiübertragung. UDP-Beispiel: Live-Streaming, VoIP oder eine normale DNS-Anfrage.

> [!success]- Teil D – Adressierung und Subnetting
> **Aufgabe 8**
>
> 1. 32 Bit und 4 Oktette.
> 2. 0 bis 255.
> 3. Netz- und Hostanteil.
> 4. Das Default Gateway leitet Pakete in andere Netze weiter.
>
> **Aufgabe 9**
>
> | Adresse | Antwort |
> |---|---|
> | `10.25.8.4` | privat |
> | `172.20.100.5` | privat |
> | `172.32.1.5` | öffentlich |
> | `192.168.80.20` | privat |
>
> **Aufgabe 10**
>
> 1. `192 = 11000000`
> 2. `224 = 11100000`
> 3. `/27 = 255.255.255.224`
> 4. `32 - 27 = 5` Hostbits
>
> **Aufgabe 11**
>
> - Maske: `255.255.255.224`
> - Blockgrösse: `256 - 224 = 32`
> - Blöcke: `0–31`, `32–63`, `64–95`, ...
> - `78` liegt im Block `64–95`.
> - Netzwerkadresse: `192.168.40.64`
> - Broadcast: `192.168.40.95`
> - Hostbereich: `192.168.40.65 – 192.168.40.94`
> - Nutzbare Hosts: `2^5 - 2 = 30`
>
> **Aufgabe 12**
>
> 1. Eine klassische MAC-Adresse hat 48 Bit und adressiert eine Netzwerkschnittstelle im lokalen Netz.
> 2. IPv6 hat 128 Bit und wurde hauptsächlich wegen des zu kleinen IPv4-Adressraums eingeführt.

> [!success]- Teil E – Projektvorgehen
> **Aufgabe 13**
>
> 1. Zum Beispiel Anzahl Mitarbeitende/Geräte, Räume und Distanzen, vorhandene Leitungen/Hardware, benötigte Dienste, Internetanschluss, Sicherheitsanforderungen und erwartetes Wachstum.
> 2. IST beschreibt die aktuelle Situation, etwa „in der neuen Filiale ist noch keine Netzwerkverkabelung vorhanden“. SOLL beschreibt das gewünschte Ergebnis, etwa „alle Arbeitsplätze und Kassen sind sicher verbunden und dokumentiert“.
> 3. Beispiele: „Bis zum Eröffnungstag haben alle sechs PCs Zugriff auf NAS und Drucker“; „Das Mitarbeiter-WLAN deckt alle Arbeitsräume ab und ist vom Kassennetz getrennt“. Ziele müssen überprüfbar sein.
> 4. Budget und Termin begrenzen die möglichen Varianten, Produkte, Ressourcen und Reihenfolge der Arbeiten.
>
> **Aufgabe 14**
>
> | Ergebnis | Phase |
> |---|---|
> | Anforderungen und IST-Aufnahme | Analyse |
> | Variantenvergleich und Netzkonzept | Konzept |
> | Termin-, Budget- und Materialplan | Planung |
> | montierte und konfigurierte Geräte | Umsetzung |
> | Testprotokoll und Abnahme | Test/Abnahme |
> | Betriebsanleitung und Übergabe | Abschluss/Betrieb |

> [!success]- Teil F – Praktisches Netzkonzept
> **Aufgabe 15 – Beispielplan**
>
> ```text
>                           INTERNET
>                               |
>                    [Router/Firewall R01]
>                       192.168.50.1/24
>                               |
>                      [Switch SW01 .10]
>            _______________|________________
>           /        /       |        \       \
>      NAS01 .20 PRN01 .40 POS01 .200 POS02 .201 AP01 .11
>                                                   )))
>                                         sechs PCs per DHCP
> ```
>
> Eine andere saubere Darstellung mit korrekten Verbindungen und Adressen ist ebenfalls richtig.
>
> **Aufgabe 16 – Beispiel**
>
> | Gerät | IP-Adresse | Maske | Gateway | Art |
> |---|---|---|---|---|
> | Router R01 | `192.168.50.1` | `/24` | Provider/WAN | statisch |
> | Switch SW01 | `192.168.50.10` | `/24` | `192.168.50.1` | statisch |
> | Access Point AP01 | `192.168.50.11` | `/24` | `192.168.50.1` | statisch |
> | NAS01 | `192.168.50.20` | `/24` | `192.168.50.1` | statisch |
> | Drucker PRN01 | `192.168.50.40` | `/24` | `192.168.50.1` | statisch |
> | Kasse POS01 | `192.168.50.200` | `/24` | `192.168.50.1` | statisch |
> | Kasse POS02 | `192.168.50.201` | `/24` | `192.168.50.1` | statisch |
> | Büro-PCs | `.100–.199` | `/24` | `192.168.50.1` | DHCP |
>
> **Aufgabe 17**
>
> 1. Zum Beispiel Router/Firewall 1×, verwaltbarer Switch 1×, Access Point 1×, NAS 1×, Festplatten passend zum NAS, Patchkabel mindestens 11×, Verlegekabel, Netzwerkdosen, Patchpanel, Rack und USV. Mengen müssen zum Plan passen.
> 2. Produkt/Modell, Anzahl, Einzelpreis, Totalpreis und Anbieter/Bezugsquelle; zusätzlich ist die Auswahlbegründung verlangt.
> 3. Zum Beispiel genügend Ports, benötigte Geschwindigkeit, VLAN-Unterstützung, PoE, SFP-Uplinks, Verwaltung oder Garantie.
>
> **Aufgabe 18**
>
> 1. Geräte, Verbindungen, Gerätenamen, IP-Adressen/Präfixe; zusätzlich etwa Räume, Ports, Kabeltyp oder Legende.
> 2. Zweck/Standort, Anschlüsse, Zugang, IP-Grundkonfiguration; zusätzlich Benutzerverwaltung, WLAN/Sicherheit, Backup, Wiederherstellung, Bedienung oder Fehlersuche.

> [!success]- Teil G – Inbetriebnahme und Fehlersuche
> **Aufgabe 19**
>
> 1. Strom, Link-LED, Kabel, Switch-Port und WLAN-Verbindung kontrollieren.
> 2. `ip address` prüft Adresse und Interface; `ip route` prüft Route und Default Gateway.
> 3. `ping -c 3 192.168.50.1` prüft die lokale Verbindung zum Router.
> 4. `ping -c 3 8.8.8.8` prüft den Internetweg ohne Namensauflösung.
> 5. `nslookup example.com` oder `dig example.com` prüft DNS.
> 6. `traceroute example.com` oder `tracepath example.com` zeigt den Paketweg.

---

# Auswertung

| Punkte | Einschätzung |
|---:|---|
| 108–120 | Sehr gut vorbereitet |
| 96–107 | Gut vorbereitet |
| 84–95 | Solide; einzelne Themen wiederholen |
| 72–83 | Grundlagen vorhanden; Lücken gezielt schliessen |
| unter 72 | Zusammenfassung nochmals durcharbeiten |

## Fehleranalyse

| Teil | Erreicht | Maximum | Wiederholen? |
|---|---:|---:|---|
| A – Architektur/Topologien |  | 12 |  |
| B – Medien/Komponenten |  | 16 |  |
| C – OSI/Protokolle |  | 20 |  |
| D – Adressierung/Subnetting |  | 24 |  |
| E – Projektvorgehen |  | 14 |  |
| F – Netzkonzept |  | 24 |  |
| G – Fehlersuche |  | 10 |  |

Zur Wiederholung: [[vorbereitung Modul 117]]
