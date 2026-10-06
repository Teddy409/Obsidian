# Prüfungsvorbereitung Modul 117 – Block 1 bis 4

**Modul:** Informatik- und Netzinfrastruktur für ein kleines Unternehmen realisieren  
**Grundlage:** `Modul-117_BL01.pdf` bis `Modul-117_BL04.pdf`  
**Ziel:** Lernzusammenfassung, Rechenhilfe, Netzwerkplanung und Prüfungsvorbereitung

> [!important]
> Lerne nicht nur Begriffe auswendig. Du musst erklären, vergleichen, einen Netzplan zeichnen, IP-Adressen sinnvoll vergeben und dein Vorgehen begründen können.

## Lernplan

| Einheit | Thema | Ziel |
|---|---|---|
| 1 | Netzwerkarten und Topologien | Varianten erklären, Vor-/Nachteile und SPOF erkennen |
| 2 | Kabel, Funk und Komponenten | Medium und Gerät passend auswählen |
| 3 | OSI, TCP/IP und Protokolle | Schichten, Geräte, Dienste und Ports zuordnen |
| 4 | IPv4, IPv6, MAC und Subnetzmaske | Adressen verstehen und Subnetze berechnen |
| 5 | Projektvorgehen | IST/SOLL, Auftrag, Budget, Zeit und Phasen erklären |
| 6 | Netzprojekt dokumentieren | Netzplan, Materialliste und Handbuch erstellen |
| 7 | Probeprüfung | Unter Zeitdruck lösen und Fehler gezielt wiederholen |

**Empfehlung:** Pro Einheit 45–60 Minuten lernen. Danach die [[Probeprüfung Modul 117]] ohne Lösungen bearbeiten.

---

# 1. Netzwerk-Grundlagen

## Was ist ein Netzwerk?

Ein Computernetzwerk verbindet mindestens zwei Geräte, damit sie Daten austauschen und gemeinsame Ressourcen nutzen können. Beispiele sind Internetzugang, Dateien, Drucker, E-Mail, Webseiten, Telefonie und Datenbanken.

**Protokoll:** Vereinbarte Sprache und Regeln, nach denen Kommunikationspartner Daten austauschen.

## Netzwerkarten nach Ausdehnung

| Art | Bedeutung | Ausdehnung | Beispiel |
|---|---|---|---|
| **PAN** | Personal Area Network | wenige Meter | Bluetooth zwischen Handy und Kopfhörer |
| **LAN** | Local Area Network | Gebäude/Standort | Firmennetz in einem Büro |
| **WLAN** | Wireless LAN | lokales Funknetz | Laptop über Access Point |
| **MAN** | Metropolitan Area Network | Stadt/Region | mehrere Schulstandorte einer Stadt |
| **WAN** | Wide Area Network | Land/Kontinent | Verbindung mehrerer Firmensitze |
| **GAN** | Global Area Network | weltweit | weltweites Unternehmensnetz |

> [!note]
> WLAN ist nur die drahtlose Verbindung im lokalen Netz. Das Internet ist die weltweite Verbindung vieler Netze. WLAN kann funktionieren, obwohl der Internetzugang ausgefallen ist.

## Grundbegriffe

- **SPOF – Single Point of Failure:** Einzelne Komponente, deren Ausfall das ganze System oder einen wichtigen Teil stoppt.
- **Redundanz:** Kritische Komponenten oder Verbindungen sind mehrfach vorhanden. Eine echte Redundanz darf nicht vom gleichen SPOF abhängig sein.
- **Backbone:** Leistungsfähige Hauptverbindung, die mehrere Netzbereiche miteinander verbindet.
- **Ethernet:** Standard für kabelgebundene lokale Netzwerke, standardisiert als IEEE 802.3.
- **Client:** Fordert einen Dienst an, zum Beispiel ein Browser.
- **Server:** Stellt einen Dienst bereit, zum Beispiel ein Web- oder Dateiserver.

## Topologien

| Topologie | Aufbau | Vorteil | Nachteil / SPOF | Typischer Einsatz |
|---|---|---|---|---|
| **Bus** | Alle Geräte an einer Hauptleitung | wenig Kabel | Hauptleitung stört alle; Fehlersuche schwierig | ältere Ethernet-Netze, CAN-Bus |
| **Linie** | Geräte hintereinander | einfacher Aufbau | Unterbruch trennt nachfolgende Geräte | Sensoren, Produktion |
| **Ring** | Jedes Gerät mit zwei Nachbarn | geordneter Datenweg | Unterbruch kann Ring stoppen | Industrie, Glasfaserringe |
| **Doppelring** | zwei unabhängige Ringe | höhere Ausfallsicherheit | teurer und komplexer | kritische Backbone-Verbindungen |
| **Stern** | alle Endgeräte an zentralem Switch | gut erweiterbar; Kabeldefekt betrifft nur ein Gerät | zentraler Switch ist SPOF | heutige LANs |
| **Baum** | mehrere Sterne hierarchisch verbunden | skalierbar und übersichtlich | Ausfall eines Hauptknotens betrifft einen ganzen Ast | Schule, grössere Firma |
| **Teilvermascht** | einige Knoten haben mehrere Wege | gute Redundanz | mehr Kabel und Konfiguration | Provider, Firmennetze |
| **Vollvermascht** | jeder Knoten mit jedem verbunden | höchste Ausfallsicherheit | sehr teuer; viele Verbindungen | kleine kritische Netze |

**Prüfungsantwort für ein kleines Unternehmen:** Meist Stern- oder Baumtopologie mit Switches. Sie ist übersichtlich, erweiterbar und gut zu warten. Kritische Switches, Router, Stromversorgung und Uplinks sollten redundant ausgelegt werden.

---

# 2. Übertragungsmedien und Netzwerkkomponenten

## Kupfer, Glasfaser und Funk

| Medium | Eigenschaften | Vorteile | Nachteile / Einsatz |
|---|---|---|---|
| **Twisted Pair** | verdrillte Kupferadern; ungeschirmt oder geschirmt | günstig, einfach, verbreitet | störanfälliger und kürzere Reichweite als Glasfaser |
| **Glasfaser / Fibre** | Lichtsignale durch Fasern | hohe Geschwindigkeit, grosse Distanz, unempfindlich gegen elektromagnetische Störungen | teurer, empfindlich bei Montage, Spezialwerkzeug |
| **WLAN** | Funkübertragung | mobil, keine Leitung zum Endgerät | Störungen, geteilte Bandbreite, Sicherheitskonfiguration nötig |
| **PowerLAN** | Daten über Stromleitungen | nutzt vorhandene Leitungen | Leistung hängt stark von Elektroinstallation und Störungen ab |

## Abschirmung bei Twisted Pair

- **Ungeschirmt (UTP):** günstiger und flexibel, aber weniger Schutz gegen elektromagnetische Störungen.
- **Geschirmt (STP/FTP):** zusätzliche Folien- oder Geflechtschirmung; sinnvoll in störungsreicher Umgebung.
- Die Schirmung muss fachgerecht installiert und geerdet werden.
- Kupfer wird für Endgeräte verwendet; Glasfaser häufig für Backbone, Gebäude- und lange Verbindungen.

## Wichtige Geräte

| Gerät | Aufgabe | OSI-Schicht |
|---|---|---:|
| **Repeater** | regeneriert ein Signal | 1 |
| **Hub** | sendet Bits an alle Ports | 1 |
| **Medienkonverter** | wandelt zum Beispiel Kupfer in Glasfaser um | 1 |
| **Netzwerkkarte** | verbindet Gerät mit dem Netz; besitzt MAC-Adresse | 1/2 |
| **Bridge** | verbindet Segmente anhand MAC-Adressen | 2 |
| **Switch** | leitet Frames anhand MAC-Adressen gezielt weiter | 2 |
| **Access Point** | verbindet WLAN-Geräte mit dem kabelgebundenen LAN | 2 |
| **Router/Gateway** | verbindet unterschiedliche IP-Netze | 3 |
| **Layer-3-Switch** | Switching und Routing | 2/3 |
| **Paketfirewall** | filtert unter anderem IP-Adressen | 3 |
| **Stateful Firewall** | verfolgt Verbindungszustände und Ports | 4 |
| **Proxy** | vermittelt Anfragen auf Anwendungsebene | 7 |
| **SFP-Modul** | steckbares Sende-/Empfangsmodul, oft für Glasfaser | 1 |

**WLAN-Repeater:** Vergrössert die Funkabdeckung, muss Daten aber erneut per Funk übertragen. Dadurch können Leistung und Stabilität sinken. Für ein Firmennetz sind verkabelte Access Points meist besser.

---

# 3. OSI- und TCP/IP-Modell

## Die sieben OSI-Schichten

| Nr. | Deutsch / Englisch | Hauptaufgabe | Beispiele |
|---:|---|---|---|
| **7** | Anwendung / Application | Netzwerkdienste für Anwendungen | HTTP, HTTPS, FTP, SMTP, DNS |
| **6** | Darstellung / Presentation | Format, Codierung, Verschlüsselung | Datenformate, TLS-Funktionen |
| **5** | Sitzung / Session | Sitzungen aufbauen, steuern, beenden | RPC |
| **4** | Transport / Transport | Ende-zu-Ende-Transport, Ports | TCP, UDP |
| **3** | Vermittlung / Network | logische Adressierung und Routing | IPv4, IPv6, ICMP, Router |
| **2** | Sicherung / Data Link | Frames, MAC-Adressen, lokaler Transport | Ethernet, Switch, Access Point |
| **1** | Bitübertragung / Physical | Bits, Signale, Kabel und Stecker | Hub, Repeater, Kupfer, Fibre |

**Merksatz:** **1 Bits → 2 MAC → 3 IP → 4 TCP/UDP → 5 Sitzung → 6 Darstellung → 7 Anwendung**

## OSI zu TCP/IP

| TCP/IP-Schicht | Entsprechende OSI-Schichten |
|---|---|
| Anwendung | 5–7 |
| Transport | 4 |
| Internet | 3 |
| Netzzugang / Link | 1–2 |

## Kapselung

Beim Senden werden von oben nach unten Steuerinformationen ergänzt:

```text
Anwendungsdaten
   ↓
TCP-Segment / UDP-Datagramm
   ↓
IP-Paket
   ↓
Ethernet-Frame
   ↓
Bits auf Kabel/Funk
```

Beim Empfänger geschieht der Vorgang umgekehrt.

## TCP und UDP

| TCP | UDP |
|---|---|
| verbindungsorientiert | verbindungslos |
| Bestätigungen und Reihenfolge | keine Zustellgarantie |
| verlorene Daten werden erneut übertragen | keine automatische Wiederholung |
| zuverlässiger, aber mehr Aufwand | schnell und geringer Overhead |
| Web, E-Mail, Dateiübertragung | Streaming, VoIP, DNS-Anfragen |

---

# 4. Netzwerkdienste, Protokolle und Ports

| Protokoll/Dienst | Aufgabe | Standard-Port |
|---|---|---:|
| **HTTP** | unverschlüsselte Webseitenübertragung | 80/TCP |
| **HTTPS** | verschlüsselte Webseitenübertragung mit TLS | 443/TCP |
| **FTP** | Dateien übertragen; Steuerkanal | 21/TCP |
| **FTP aktiv** | Datenkanal vom Server | 20/TCP |
| **SMTP** | E-Mails versenden/weiterleiten | 25/TCP |
| **POP3** | E-Mails vom Server abrufen | 110/TCP |
| **IMAP** | E-Mails auf dem Server verwalten | 143/TCP |
| **DNS** | Namen in IP-Adressen und umgekehrt auflösen | 53/UDP und TCP |
| **DHCP** | IP-Konfiguration automatisch vergeben | 67/68 UDP |
| **SSH** | verschlüsselte Fernverwaltung | 22/TCP |

Weitere wichtige Protokolle:

- **ARP:** Ermittelt im lokalen IPv4-Netz die MAC-Adresse zu einer IP-Adresse. Ein ARP Request fragt, die ARP Response antwortet; Zuordnungen landen im ARP Cache.
- **IP:** Transportiert Pakete anhand logischer IP-Adressen zwischen Netzen.
- **ICMP:** Kontroll- und Fehlermeldungen; wird zum Beispiel von `ping` verwendet.
- **NFS/Dateidienst:** Stellt Dateien über das Netzwerk bereit.
- **VoIP:** Überträgt Sprache über ein IP-Netz.

---

# 5. MAC-, IPv4- und IPv6-Adressen

## MAC-Adresse

- Physikalische Adresse einer Netzwerkschnittstelle.
- Klassisch **48 Bit = 6 Byte**.
- Hexadezimale Schreibweise, zum Beispiel `00:1A:2B:3C:4D:5E`.
- Die ersten 3 Byte kennzeichnen den Hersteller (OUI/Vendor), die letzten 3 Byte das Gerät.
- Switches verwenden MAC-Adressen zur Weiterleitung im lokalen Netz.

## IPv4

- **32 Bit**, aufgeteilt in **4 Oktette**.
- Jedes Oktett hat einen Dezimalwert von **0 bis 255**.
- Beispiel: `192.168.10.37`.
- Die Subnetzmaske trennt **Netzanteil** und **Hostanteil**.
- Router verwenden IP-Adressen zur Weiterleitung zwischen Netzen.

## Private IPv4-Bereiche

| Bereich | CIDR |
|---|---:|
| `10.0.0.0 – 10.255.255.255` | `/8` |
| `172.16.0.0 – 172.31.255.255` | `/12` |
| `192.168.0.0 – 192.168.255.255` | `/16` |

Private Adressen werden im öffentlichen Internet nicht geroutet. Der Router übersetzt sie für den Internetzugang normalerweise mit NAT/PAT auf eine öffentliche Adresse.

## IPv6

- **128 Bit** statt 32 Bit.
- Sehr grosser Adressraum: ungefähr `3,4 × 10^38` Adressen.
- Hexadezimale Schreibweise, zum Beispiel `2001:db8::1`.
- Entwickelt, weil der IPv4-Adressraum begrenzt ist.

## Classful und CIDR

Früher wurden IPv4-Adressen in feste Klassen A, B und C eingeteilt. Heute wird **CIDR (Classless Inter-Domain Routing)** mit Präfixen wie `/24` oder `/27` verwendet. Das Präfix nennt die Anzahl Netzbits.

---

# 6. Subnetzmaske sicher berechnen

## Binärwerte eines Oktetts

| Bitwert | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|---|---:|---:|---:|---:|---:|---:|---:|---:|

Beispiel:

```text
192 = 128 + 64             = 11000000
168 = 128 + 32 + 8         = 10101000
224 = 128 + 64 + 32        = 11100000
```

## Wichtige Präfixe

| Präfix | Subnetzmaske | Adressen | Nutzbare Hosts | Blockgrösse |
|---:|---|---:|---:|---:|
| `/24` | `255.255.255.0` | 256 | 254 | 256 |
| `/25` | `255.255.255.128` | 128 | 126 | 128 |
| `/26` | `255.255.255.192` | 64 | 62 | 64 |
| `/27` | `255.255.255.224` | 32 | 30 | 32 |
| `/28` | `255.255.255.240` | 16 | 14 | 16 |
| `/29` | `255.255.255.248` | 8 | 6 | 8 |
| `/30` | `255.255.255.252` | 4 | 2 | 4 |

**Formeln:**

```text
Hostbits = 32 - Präfix
Anzahl Adressen = 2^Hostbits
Nutzbare Hosts = 2^Hostbits - 2
Blockgrösse = 256 - Wert des interessanten Masken-Oktetts
```

Die zwei nicht nutzbaren Adressen sind normalerweise die **Netzwerkadresse** und die **Broadcast-Adresse**.

## Rechenweg am Beispiel `192.168.20.75/27`

1. `/27` entspricht `255.255.255.224`.
2. Hostbits: `32 - 27 = 5`.
3. Adressen: `2^5 = 32`, davon `30` nutzbar.
4. Blockgrösse: `256 - 224 = 32`.
5. Blöcke im letzten Oktett: `0, 32, 64, 96, 128, 160, 192, 224`.
6. `75` liegt im Block `64–95`.

| Gesucht | Ergebnis |
|---|---|
| Netzwerkadresse | `192.168.20.64` |
| erster Host | `192.168.20.65` |
| letzter Host | `192.168.20.94` |
| Broadcast | `192.168.20.95` |
| nutzbare Hosts | 30 |

## Gleiches Subnetz prüfen

Bei `/24` müssen die ersten drei Oktette gleich sein. Bei anderen Präfixen zuerst den Block bestimmen. Zwei Adressen gehören nur dann zum gleichen Subnetz, wenn sie zwischen derselben Netzwerk- und Broadcast-Adresse liegen.

---

# 7. Sinnvolle IP-Adressplanung

Ein klares Schema erleichtert Betrieb, Dokumentation, Firewall-Regeln und Fehlersuche.

Beispiel für `192.168.10.0/24`:

| Bereich | Verwendung |
|---|---|
| `.1 – .19` | Router, Firewall, Switches, Access Points |
| `.20 – .39` | Management-Schnittstellen |
| `.40 – .59` | Server |
| `.60 – .69` | NAS und Backup |
| `.70 – .99` | Drucker, Kameras, Spezialgeräte |
| `.100 – .200` | DHCP-Bereich für Clients |
| `.201 – .249` | Reserve |
| `.250 – .254` | besondere Infrastruktur/Reserve |

Regeln:

- Netzwerkadresse und Broadcast nie an Geräte vergeben.
- Jede Geräte-IP muss eindeutig sein.
- Alle Geräte im gleichen Subnetz verwenden dieselbe Maske.
- Das Default Gateway liegt im lokalen Netz und zeigt zum Router.
- Statische Infrastrukturadressen ausserhalb des DHCP-Bereichs planen.
- Gerät, Systemname, IP, MAC, Standort und Anschluss dokumentieren.

---

# 8. Netzwerkplan zeichnen

Ein guter physischer/logischer Netzplan enthält:

- Internet/WAN-Verbindung
- Router/Firewall und Default Gateway
- Switches und Access Points
- Server, NAS, Drucker und Clients
- Kabel- oder Funkverbindungen
- Gerätenamen, IP-Adressen und Präfix/Subnetzmaske
- bei Bedarf Raum, Portnummer, VLAN und Kabeltyp
- Legende und klare Leserichtung

## Musterplan

```text
                               INTERNET
                                   |
                         [Router/Firewall R01]
                         IP: 192.168.10.1/24
                                   |
                         [Managed Switch SW01]
                         IP: 192.168.10.10/24
                    _________|___________
                   /         |           \
          [Server SRV01] [Drucker PRN01] [Access Point AP01]
          192.168.10.40  192.168.10.70   192.168.10.11
                   |                         ))) WLAN
             [NAS01 .60]                  Laptop .120
                                             Handy DHCP
```

**Prüfungstipp:** Erst Geräte platzieren, dann Verbindungen zeichnen, danach Namen und IP-Adressen eintragen. Zum Schluss prüfen: doppelte IP, falscher Bereich, fehlendes Gateway, fehlende Maske?

---

# 9. Vorgehen bei einem Netzwerkprojekt

## Was ist ein Projekt?

Ein Projekt ist einmalig, zeitlich und finanziell begrenzt, verfolgt definierte Ziele und wird schrittweise mit klaren Rollen und Aufgaben durchgeführt.

## Projekt-Vorphase

Vor der technischen Lösung müssen die Anforderungen verstanden werden:

1. **Firmenporträt:** Branche, Standorte, Mitarbeitende, Räume, Arbeitsweise.
2. **Projektauftrag:** Was soll erreicht und geliefert werden?
3. **Projektziele:** konkret und überprüfbar formulieren.
4. **Budget:** Wie viel Geld steht zur Verfügung?
5. **Zeit:** Termine, Abhängigkeiten und Abgabe.
6. **IST-Zustand:** Was ist heute vorhanden? Was funktioniert oder fehlt?
7. **SOLL-Zustand:** Wie soll die Lösung nach dem Projekt aussehen?
8. **Anforderungen:** Muss-, Soll- und Kann-Anforderungen priorisieren.

## Typische Projektphasen

| Phase | Wichtige Fragen / Tätigkeiten |
|---|---|
| **Initialisierung** | Auftrag, Ziele, Rollen und Rahmen klären |
| **Analyse** | IST aufnehmen, Bedürfnisse und Risiken erfassen |
| **Konzept** | Varianten, Topologie, IP-Plan und Produkte vergleichen |
| **Planung** | Termine, Budget, Material, Zuständigkeiten und Tests planen |
| **Umsetzung** | Hardware montieren und Geräte konfigurieren |
| **Test/Abnahme** | Funktion, Leistung und Sicherheit prüfen; Mängel beheben |
| **Betrieb/Abschluss** | dokumentieren, übergeben, schulen und überwachen |

## Entscheidungen begründen

Eine gute Entscheidung nennt:

- Anforderungen und Ausschlusskriterien
- mindestens zwei Varianten
- Kosten, Nutzen, Risiken und Folgekosten
- technische Eignung und Erweiterbarkeit
- nachvollziehbare Empfehlung

---

# 10. Pflichtunterlagen des Installationsprojekts

## Netzplan

Layout auf Büro-Skizze mit Verbindungen, IP-Adressen, Gerätenamen und Deklaration.

## Budgetplan

| Position | Produkt | Anzahl | Einzelpreis | Total | Anbieter | Begründung |
|---|---|---:|---:|---:|---|---|
| Beispiel | Managed Switch | 1 | CHF 180 | CHF 180 | Händler | genügend Ports, VLAN-fähig |

Nur verlangte Kosten aufnehmen. In der PDF werden für den Budgetplan Hardwarekosten, Bezugsquelle und Auswahlgrund verlangt.

## Projektplan

Phasen, Tätigkeiten, Termine, Verantwortliche, Abhängigkeiten und Ergebnisse aufführen.

## Materialliste

Neue Hardware und benötigtes Installationsmaterial, zum Beispiel:

- Router/Firewall, Switch, Access Point, NAS
- Patchkabel, Verlegekabel, Patchpanel, Dosen und Stecker
- SFP-Module und Glasfaserkabel, falls benötigt
- Rack, Stromversorgung und Beschriftungsmaterial
- Anzahl, Modell, technische Eigenschaft und Verwendungszweck

## Betriebsanleitung und Konfigurationshandbuch

Für eine gekaufte Komponente dokumentieren:

- Produkt, Zweck, Standort und Anschlüsse
- Zugang und Grundkonfiguration
- Benutzer oder Administrator einrichten
- IP-, WLAN- und Sicherheitseinstellungen
- Backup und Wiederherstellung
- normale Bedienung und häufige Fehler
- Versionsstand, Datum und verantwortliche Person

> [!warning]
> Keine echten Passwörter in die allgemeine Dokumentation schreiben. Zugangsdaten sicher und getrennt verwalten.

---

# 11. Inbetriebnahme, Funktionskontrolle und Fehlersuche

## Sinnvolle Prüfreihenfolge

1. **Physisch:** Strom, LEDs, Kabel, Port und WLAN-Signal.
2. **Lokale Konfiguration:** eigene IP, Maske, Gateway und DNS.
3. **Loopback:** `ping 127.0.0.1`.
4. **Gateway:** Router im eigenen Netz anpingen.
5. **Internet per IP:** zum Beispiel `ping 8.8.8.8`.
6. **DNS:** Namen mit `nslookup` oder `dig` auflösen.
7. **Route:** mit `traceroute` oder `tracepath` den Weg prüfen.
8. **Dienst:** Anwendung und Port testen.
9. **Dokumentieren:** Ursache, Änderung und Resultat festhalten.

## Nützliche Befehle

| Befehl | Zweck |
|---|---|
| `ip address` | IP-Adressen und Interfaces anzeigen |
| `ip route` | Routingtabelle und Default Gateway anzeigen |
| `ping -c 3 <IP>` | Erreichbarkeit prüfen |
| `ip neigh` | ARP-/Nachbartabelle anzeigen |
| `nslookup <name>` / `dig <name>` | DNS-Auflösung prüfen |
| `traceroute <ziel>` / `tracepath <ziel>` | Paketweg anzeigen |
| `ss -tulpen` | lokale Ports und Verbindungen anzeigen |
| `nmap -sV <IP>` | erreichbare Dienste untersuchen, nur mit Erlaubnis |

## Abnahme

- Erfüllt die Lösung alle Muss-Anforderungen?
- Funktionieren LAN, WLAN, Internet, DNS, Drucker und Server?
- Stimmen IP-Plan, Gerätenamen und Netzplan mit der Realität überein?
- Wurden Leistung, Sicherheit, Updates und Backups geprüft?
- Sind Tests und Mängel protokolliert?
- Wurden Betrieb und Dokumentation übergeben?

---

# 12. Prüfung-Checkliste

Du bist bereit, wenn du ohne Hilfe:

- [ ] LAN, WLAN, MAN, WAN und GAN erklären kannst.
- [ ] sieben Topologien mit Vorteil, Nachteil und SPOF vergleichen kannst.
- [ ] Kupfer, Glasfaser und WLAN sinnvoll auswählst.
- [ ] Hub, Switch, Router, Access Point, Firewall und Proxy unterscheidest.
- [ ] die sieben OSI-Schichten in Reihenfolge kennst.
- [ ] TCP, UDP, ARP, IP, ICMP und DNS erklären kannst.
- [ ] wichtige Dienste und Ports zuordnest.
- [ ] MAC, IPv4, IPv6 sowie private und öffentliche IP unterscheidest.
- [ ] `/24` bis `/30` in Maske, Hostzahl und Blockgrösse umrechnest.
- [ ] Netzwerk-, Host- und Broadcast-Adresse berechnest.
- [ ] einen sauberen Netzwerkplan mit IP-Schema zeichnest.
- [ ] IST, SOLL, Auftrag, Budget, Zeit und Anforderungen erklärst.
- [ ] Netzplan, Budgetplan, Projektplan, Materialliste und Handbuch erstellen kannst.
- [ ] Netzwerkfehler systematisch von Schicht 1 nach oben suchst.

## Verknüpfte Notizen

- [[00 Netzwerk Lernübersicht]]
- [[Netzwerk Grunlagen]]
- [[Der weg zu Netzwerke]]
- [[Topoligie Netzwerke]]
- [[OSI Modelle]]
- [[Dezimal Bit]]
- [[IP submaske verstehen tabelle]]
- [[aufgabe]]
- [[befehle und config 1]]
- [[Probeprüfung Modul 117]]
