# Praxisaufgabe – Netzwerkplan erstellen

**Ziel:** Das eigene Netzwerk scannen und anschliessend als übersichtlichen Netzwerkplan zeichnen.

## 1. Schritt – Netzwerk scannen mit Advanced IP Scanner

Mit dem Tool **[Advanced IP Scanner](https://www.advanced-ip-scanner.com/de/)** lässt sich ein Netzwerkbereich in Sekunden scannen. Man gibt den IP-Bereich ein (z. B. `192.168.56.1-254`) und erhält als Ergebnis alle gefundenen Geräte mit ihrer **IP-Adresse** und **MAC-Adresse**.

![](Pasted%20image%2020260924202124.png)

*Scan-Bereich eingeben und auf „Scannen" klicken:*

![](Pasted%20image%2020260924204204.png)

## 2. Schritt – Netzwerkplan zeichnen mit yEd Graph Editor

Mit dem kostenlosen **yEd Graph Editor** lässt sich der Netzwerkplan grafisch zeichnen. In der Palette rechts gibt es die Kategorie **„Computer-Netzwerk"** mit fertigen Symbolen (PC, Switch, Server, Drucker, Internet/Cloud).

**Vorgehen:**
1. Gewünschtes Symbol (z. B. PC oder Switch) aus der Palette auf die Zeichenfläche ziehen.
2. Symbole durch Anklicken und Ziehen mit **Linien verbinden**.
3. Über das **Eigenschaften-Fenster** (Doppelklick auf ein Element) Text, Farbe und Grösse anpassen.

![](Pasted%20image%2020260924204754.png)

![](Pasted%20image%2020260924204811.png)

![](Pasted%20image%2020260924204917.png)

## 3. Ergebnis – Netzwerkplan

```text
                         INTERNET
                            |
                            |
                    +----------------+
                    |     Router     |
                    | 192.168.1.1    |
                    +----------------+
                      /      |      \
                    WLAN    LAN     WLAN
                    /        |        \
          +---------+   +---------+   +---------+
          | Laptop  |   |  PC     |   | Handy   |
          | .20     |   | .30     |   | .40     |
          +---------+   +---------+   +---------+
                            |
                        +---------+
                        | Drucker |
                        | .50     |
                        +---------+
```

---

## 🔗 Verknüpfungen zum Lernen

- [[Netzwerk Grunlagen|Netzwerk-Grundlagen]]
- [[IP submaske verstehen tabelle|IP-Adressen & Subnetzmaske]]
- [[Topoligie Netzwerke|Topologien]]
- [[befehle und config 1|Netzwerk-Befehle]]
