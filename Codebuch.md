##Codebuch Modedesigner*inen und Luxusmarken##
Codebuch Stand 2023-06, aktualisiert 2023-11
erstellt von Fashionistas (cp071@hdm-stuttgart.de)


## Inhalt
- Edges.csv (Edgelist) 
- Nodes.csv (Nodelist)
- CodebuchFashionistas.md (Codierung der Datensätze)



## Ursprung und Datenerhebung
Wir haben den Datensatz unter den Modedesigner*innen in der Luxusmarkenbranche erhoben.

Das Netzwerk ist ein *gerichtetes Akteursnetzwerk*. Es wurden vier getrennte Fragen erhoben:


**Forschungsfragen**

1a) Wie sind bekannte Modebrands mit Fashion Designer*innen verbunden?

1b) Welche Wechsel gab es während der Laufbahn der Designer*innen?

1c) Welche Musen haben ihr berufliches Schaffen während ihrer Karriere beeinflusst?

1d)Gibt es typische Eigenschaften von Designer*innen und Musen?

**Hinweis**

- NA: Fehlende Werte werden als 999 codiert.

**Netzwerke**

- ein Gesamtnetzwerk (d)
- drei **Teilnetzwerke** nach den Positionen (assistant, director und founder)
- ein Teilnetzwerk (muse) erstellt, welches die Verbindungen zwischen Designer*innnen und Musen visualisiert 

# EDGE-Attribute


**from**

initiierender Knoten, in diesem Fall: Designer/in wechselte von einer zur anderen Marke.

**to**

erhaltender Knoten, in diesem Fall: Marke , für die ein/e Designer*in arbeitet.


**position**

Designer*innen Rang innerhalb einer Brand

1 = Jeglicher unterer Rang oder Design Assistant Design Assistant
2 = Creative Director
3 = Founder

**year**

Jahr, in dem der Wechsel stattfand.






# NODE-Attribute  
  
**id**  

(eindeutige Codierung des Knoten )
klare Codierung durch Abkürzung der Namen der Knoten, jede ID entspricht einem Designer. Knoten für die Musen (Models) werden noch erhoben. Hierbei untersuchen wir, ob die Musen zu der neuen Modemarke mit gewechselt sid.

**name**

voller Name


**sex** 

1 = weiblich  
2 = männlich  
3 = divers
  

**birthyear**   

Geburtsjahr des Knotens  


**main workplace**

Sitz der Brand oder Hauptarbeitsplatz des Knotens

de = Deutschland,
usa = Amerika,
it = Italien,
fr = Frankreich, 
gb = England,
jap = Japan,
dr = Dominikanische Republik,
ven = Venezuela,
bra = Brasilien,
wal = Wales,
sp = Spanien
b = Belgien

**type**

1 = muse
2 = brand
3 = designer



**scholar**

Abschlussart des Designers 

1 = *talent* : Der/Die Designer*in hat bis auf seine kreative Ader keinen Abschluss.
2 = *internship/work experience* : Der/Die Designer*in hatte eine Art Ausbildung bei einem Mentor oder praktische Erfahrungen in der Modebranche gesammelt.
3 = *degree* Der/Die Designer*in hat eine Modeschule oder vergleichbares besucht.


**sexuality**  

1 = heterosexual: Der/Die Designer*in ist heterosexuell
2 = homosexual: Der/Die Designer*in ist homosexuell   
3 = bisexual : Der/Die Designer*in ist bisexuell


**transfer**
1 = Der/Die Deswigner*in hat direkt seine eigene Marke gegründet
2 = Der/Die Designer*in hat die Marke ein mal gewechselt
3 = Der/Die Designer*in hat die Marke zwei mal gewechselt
4 = Die Marke wurde drei oder mehrmals gewechselt


**value**

Designervermögen/ Markenwert

1 = 1 - 50 Mio. Dollar
2 = 55 - 100 Mio. Dollar
3 = 105 - 500 Mio. Dollar
4 = 505 - 1 Mrd. Dollar
