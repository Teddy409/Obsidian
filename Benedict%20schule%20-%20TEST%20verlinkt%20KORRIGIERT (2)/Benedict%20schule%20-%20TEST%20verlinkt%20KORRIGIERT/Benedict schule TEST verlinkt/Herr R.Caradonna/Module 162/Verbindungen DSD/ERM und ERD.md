**ERM** und **ERD** gehören zur Planung von Datenbanken.
Entitäten (Tabellen) werden mit Rechtecken, Attribute mit Ovalen dargestellt. Primärschlüssel werden unterstrichen!​

![[Pasted image 20260912130941.png]]


Das ERM ist die **Idee bzw. das Modell** hinter einer Datenbank. Du überlegst dabei:

- Welche Dinge gibt es?
- Welche Eigenschaften haben diese Dinge?
- Wie hängen sie miteinander zusammen?

Beispiel Schule:

- **Schüler**
- **Lehrer**
- **Klasse**

### Das ERD ist einfach die grafische Zeichnung vom ERM

+----------------+
|    SCHÜLER     |
+----------------+
| Schüler_ID     |
| Name           |
| Vorname        |
+----------------+
        |
        | besucht
        |
        v
+----------------+
|     KLASSE     |
+----------------+
| Klassen_ID     |
| Klassenname    |
+----------------+



# Programm
- Programmziele:​
    
- Abteilung – Mitarbeiter – Projekt, Lösungen:​
    - 
- ERM / ERD​
    
- DSD (Datenstrukturdiagram)​
    
- Relationenschreibweise​
    
- Buchhandlung​
    
- ERM / ERD​
    
- DSD (Datenstrukturdiagram)​
    
- Relationenschreibweise​
    
- Repetition, Prüfungsdaten, Prüfungsziele​
    
- Access kennenlernen 'Kontaktdatenbank'​

**-Fremdschlüssel**

- Abteilungs ( abt.nr Name, Ort)
- Mitarbeiter (persnr, name, gebdatum,adresse,gehalt,tätigkeit ,abtnr,projnr)
- Projekte ( Proj.Nr P beginn,pende,stunden,persnr))

**Primärschlüssel**

- **Abteilung:** `abtnr`
- **Mitarbeiter:** `persnr`
- **Projekt:** `projnr`
 





|Tabelle|Primärschlüssel|Fremdschlüssel|
|---|---|---|
|**Abteilung**|`abtnr`|–|
|**Mitarbeiter**|`persnr`|`abtnr`|
|**Projekt**|`projnr`|–|
|**Mitarbeiter_Projekt**|`persnr + projnr`|`persnr`, `projnr`|


![[Pasted image 20260912132601.png]]




**Eine Abteilung hat viele Mitarbeiter.**

```
Abteilung
   1
   |
   n
Mitarbeiter
```

`1:m` würde grundsätzlich dasselbe bedeuten wie `1:n` — **m und n stehen beide für „viele“**.


![[Pasted image 20260912133713.png]]



## **Ein Autor kann mehrere Bücher schreiben, und ein Buch kann auch mehrere Autoren haben.**





---

## 🔗 Verknüpfungen zum Lernen

- [[Verbindungen DSD/Daten und Datenanalyse|Datenbank-Grundlagen, Primär-/Fremdschlüssel]]
- [[Verbindungen DSD/MS Access|Beziehungen in Access]]
- [[Pr#U00fcfungen|Prüfungsziele]]
