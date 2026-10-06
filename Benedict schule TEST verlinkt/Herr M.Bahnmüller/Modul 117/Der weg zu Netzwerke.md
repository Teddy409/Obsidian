Das Internet ist das grösste GAN der Welt, es verbindet LAN WAN GANs und MANs , auch als **Peering** points gennannt



Daten auf jedem einzelnen system verfügbar.
Datenaustausch via:
Lochkraten
magnetböänder
disketten

ein IBM Grossrechner ender der 1950r jahre, 
Ender der 1960er jahre . 
Auftrag der ARPA (advanced Research Project Agency) an universitätet und computerhersteller zur konzeption eines redunanten Datennetzes.
- vermeidung eine SPOF
- testlauf halben Dutzenden vernetzter systeme name ARPANET
- verbindung über telnetz circuit switching
- verbindung via tel netz packet switching
- 



TCP / IP 
- ein protokoll ist eine sprache kommunikationpartner einigen

- protokolfamilie
- Transmission control protocol 
- internet protocol

familie

- Arp
- TCP /IP
- IPX/SPX
- OSI 
- DECnet


ETHERNET

- verbindungen von computersysteme innerhalb eines standort
- 1970 IBM und Xerox beginnen mit der entwicklung von lokalen netzwerk technologien
- 1973 ethernet entstanden 
- standardisierung als IEEE 802.3


COMPUTERNETZWERK

###### Local Area Network LAN

Ein LAN verbindet Geräte in einem **kleinen Bereich**, zum Beispiel in einem Haus, einer Schule oder einem Büro. Dadurch können die Geräte miteinander kommunizieren.

PC ─────┐
        │
Laptop ─┼── Switch/Router ─── Internet
        │
Drucker ┘

###### **WAN** steht für **Wide Area Network**, auf Deutsch **Weitverkehrsnetz**.

Ein WAN verbindet Netzwerke über **große Entfernungen** miteinander, zum Beispiel zwischen Städten, Ländern oder Kontinenten.
Dein Netzwerk zuhause ist ein **LAN**. Das Schulnetzwerk ist auch ein **LAN**. Wenn beide über das Internet miteinander verbunden sind, läuft die Verbindung über ein **WAN**.

###### **GAN** kann im Netzwerk-Kontext für **Global Area Network** stehen.

Ein GAN verbindet Netzwerke über **sehr große Entfernungen weltweit** miteinander.
Kurz gesagt: **LAN = lokal, WAN = weit, GAN = global.**

###### **MAN** steht für **Metropolitan Area Network**.
Ein MAN verbindet mehrere Netzwerke innerhalb einer **Stadt oder größeren Region**.

Schule A ──┐
           │
Schule B ──┼── MAN der Stadt
           │
Bibliothek ┘


##### Router

Router werden auch als Gateway bezeichnet

![](Pasted%20image%2020260927194356.png)

###### Ein **physisches Netzwerkdiagramm** zeigt, **wie die Geräte in echt miteinander verbunden sind**.

![](Pasted%20image%2020260927195150.png)




###### World Wide Web

- Client web browser
- ziel uniform ressource locator UR
- server webserver
- übertragung via HTP hypertext transer protocol Port80 tcp
- sichere variante HTTTPS secure socket layer oder TLS transportt layer security




###### Netzwerk anwendung File Tranfer Protocol FTP

- client: FTP (filezile)
- server FTP server
- dient übertragen von datei 
- 
verwaltungskanal 21/tcp und einen datenkanal 

- active 20/tcp verbindungsaufbau vom server
- passive zufälliger high port (<1023)verbindungsaufbau vom client

###### Email
- client: outlook thunderbird
- server ms exchance server postfix senmail
- simple mail transer protocol (smtp port 25/tcp)
- post office protocol pop3 110/tcp
- internet Mail application protocol IMAP4 143/tcp
- ![](Pasted%20image%2020260927204112.png)


###### Datenbank Anwendungen 


- SQL wichtigse datenbank
- live chat 
- ermöglict austausch von nachrichten in echtzeit
- bsp skype jabber online rollenspiele


###### Voice over IP

- ersetzt das alte telefonnetz public switched telephone 



###### Datei und druckdienste
- linux network file system
- druckerfreibgabe über netzwerk
- 

###### Bus Topologie 

- eterneht wurde afangs als bus 
- mediium koaxialkabel mit 50 OHM endwiederstand
- immernoch heute logischer bus
- problem troubelsshooting



###### TCP/IP adress resolituon protocol

ARP findet heraus, welche MAC-Adresse zu einer bestimmten IP-Adresse gehört. IP adress = MAC adressse 192.168.1.5 → 00:1A:2B:3C:4D:5E

ARP request = anfrage 
ARP response = antwort vm zielsystem 

jede IP kommunikation nutzt ein absender sourche und destionation empfänge radresse 
IP pakete erfordern router , um zwischen subnetzten transportier zu werde

UDP User data group protokoll

ARP = adress Resolution protocol 
	ist für dic auflösung von IP adressen in Mac zuständig

	Reqquest -- anfrage zur auflsung
	Response -- antwort vom zielsystem
	Cache speichert mappings


![361](Screenshot%202026-10-01%20132932.png)

---

## 🔗 Verknüpfungen zum Lernen

- [[Netzwerk Grunlagen|Netzwerk-Grundlagen]]
- [[Topoligie Netzwerke|Topologien]]
- [[OSI Modelle|OSI-Modell & Protokolle]]
- [[IP submaske verstehen tabelle|IPv4 & Subnetzmaske]]
