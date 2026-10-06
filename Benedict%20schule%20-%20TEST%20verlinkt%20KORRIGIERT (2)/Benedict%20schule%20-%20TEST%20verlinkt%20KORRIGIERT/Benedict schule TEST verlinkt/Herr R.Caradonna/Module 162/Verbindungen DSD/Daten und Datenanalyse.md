
```
- Microsoft Teams
- prüfunungen 26.9 nur therorisch und ein 31.10.2026 praktisch
- 
```


# Presäntation Datenbank

## Was ist eine Datenbank

- eine Datenbank ist nur aus einer Tabelle .
	
![[Pasted image 20260905135349.png]]


## Beziehungen  von fremdschlüssel zum Primärschlüssel


- Kombination der beiden Attribute "MNR", "PROJ-NR" den Datensatz eindeutig identifizieren
- Wird eine Bestellung mit einer Preisliste kombiniert, kann der Wert der Bestellung ermittelt werden.​Verknüpfende Beziehungen sind sehr häufig in Datenbanken zu finden und werden uns später noch stark beschäftigen.​
- mc = multiple c= conditional mc >0  und m>1
- 1:n Beziehung​ der Kunde macht mehrere bestellung, kundenummer bleibt gleich aber die bestellung ändert.

![[Pasted image 20260905141103.png]]

### DSD tabelle 

![[Pasted image 20260905150117.png]]

- Kunden (Ku_NR, Name, Vorname, Adresse, PLZ, Ort, Land, Telefon)
- ​Auftrag (Auf_NR, Ku_NR, Datum)​
	Bestellzeile (Best_NR, Auf_NR, Art_NR, Menge)​
	Artikel (Art_NR, Art_Grup_NR, Lief_NR, Verkaufspreis)​
	Artikelgruppen (Art_Grup_NR, Artikelgruppe)​
	Lieferanten (Lief_NR, Lieferant, Adresse, PLZ, Ort, Land, E-Mail)​


# Erklären 
Ein Primärschlüssel ist eine eindeutige Kennzeichnung für einen Datensatz. Er sorgt dafür, dass jeder Eintrag in einer Tabelle klar unterschieden werden kann. Zum Beispiel hat jeder Kunde eine eigene Kundennummer.

Ein Fremdschlüssel steht in einer anderen Tabelle und verweist auf diesen Primärschlüssel. Damit werden zwei Tabellen miteinander verbunden.

Wenn also in der Tabelle Kunden die Kundennummer 2 zu Huber gehört und in der Tabelle Projekte bei einem Projekt ebenfalls die Kundennummer 2 steht, bedeutet das: Dieses Projekt gehört zu Huber.

Kurz gesagt: Der Primärschlüssel kennzeichnet einen Datensatz eindeutig. Der Fremdschlüssel verbindet diesen Datensatz mit einem Datensatz aus einer anderen Tabelle.



---

## 🔗 Verknüpfungen zum Lernen

- [[Verbindungen DSD/ERM und ERD|ERM / ERD – Datenbank planen]]
- [[Verbindungen DSD/MS Access|MS Access – Beziehungen umsetzen]]
- [[Pr#U00fcfungen|Prüfungsziele]]
- [[Repetitone|Repetition]]
