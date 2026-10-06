
ICT buech seite 19, 39 , 43

Gültigkeits regel nochmal anschauen


**Tabelle im buch seite 16 ICT power User**

Nachschlag ASSistent , tabelle MItarbeiter. Klicke auf dem pfeil Kurzer Text dan nachschlag Assistent.


untere Tabelle vom Access 
ALLGEMEIN/NACHSCHLAGEN



Bei Beziehungen in Access sind vor allem **5 Dinge wichtig**:

1. **Die richtigen Felder verbinden.**  
    Du verbindest normalerweise einen **Primärschlüssel** mit dem passenden **Fremdschlüssel**.  
    Beispiel: `Customers.Customer ID` → `Orders.Customer ID`.
2. **Die Felder müssen dasselbe bedeuten.**  
    Nicht einfach irgendeine ID mit irgendeiner ID verbinden.  
    `Customer ID` gehört zu `Customer ID`, nicht zu `Order ID`.
3. **Die Datentypen müssen zusammenpassen.**  
    Wenn der Primärschlüssel eine Zahl ist, muss der Fremdschlüssel ebenfalls ein kompatibler Zahlentyp sein.
4. **Auf 1 und n achten.**  
    Die **1-Seite** ist normalerweise die Tabelle mit dem eindeutigen Primärschlüssel.  
    Die **n-Seite** ist die Tabelle, in der derselbe Wert mehrfach vorkommen darf.
    
    Beispiel:  
    `Customers 1 ─── ∞ Orders`  
    Ein Kunde kann mehrere Bestellungen haben.
    
5. **Referentielle Integrität verwenden.**  
    Damit verhindert Access ungültige Verknüpfungen. Eine Bestellung soll zum Beispiel nicht auf eine `Customer ID` zeigen, die gar nicht existiert.

Ein sehr guter Prüftrick ist dieser Satz:

> **„Ein ___ kann mehrere ___ haben.“**

Zum Beispiel:

> Ein Kunde kann mehrere Telefonnummern haben.

Dann weißt du sofort:

`Customers 1 ─── ∞ Phone Numbers`

Und noch ein wichtiger Punkt: Bei einer **1:n-Beziehung liegt der Fremdschlüssel meistens auf der n-Seite**.

Also bei:

`Customers 1 ─── ∞ Orders`

liegt `Customer ID` als Fremdschlüssel in `Orders`.

Wenn du willst, kann ich dir als Nächstes eine **kleine Access-Regelkarte mit 1:1, 1:n und n:m** machen, die du für die Prüfung lernen kannst.

---

## 🔗 Verknüpfungen zum Lernen

- [[Verbindungen DSD/Daten und Datenanalyse|Primär- & Fremdschlüssel]]
- [[Verbindungen DSD/ERM und ERD|ERM / ERD & Beziehungen]]
- [[Repetitone|Repetition]]
