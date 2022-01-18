# Datensatz 25 reichste Youtuber

Codebuch Stand 2022-01 erstellt von Florian Striegl, Julia Dusemond, Lina Quotschalla, Pascal Eichner und Jessica Schreiner
Inhalt

Edges_youtuber.csv (Edgelist)
Nodes_youtuber.csv (Nodelist)
Codebuch_youtuber.md (Codierung der Datensätze)

## Ursprung und Datenerhebung

Wir haben den Datensatz aus dem Vermögenmagazin der reichsten Youtuber sowie der Socialblade- Liste der Top 100 Youtube-Channels Deutschlands erhoben. Für unser Projekt analysieren wir die Top 25, deren Verbindungen und Einkommensquellen (aus welchen Bereichen auch außerhalb von Youtube z.B. Musik).

Das Netzwerk ist ein ungerichtetes two-mode Akteursnetzwerk.

## EDGE-Attribute

from ->  id des Youtubers/der Einnahmequelle(n), in ein bzw. zwei Buchstaben z.B. Simon Unge -> su

to -> type, Youtuber (0) , Einkommensquellen (1) und Organisationen (Management) (2)

relation 1 = Zusammenarbeit (Erscheinen zusammen in mind. 1 Video), 2 = Bei welcher Organisation ist die:der Youtuber:in (Management) 3 = Welche Einnahmequellen hat die:der Youtuber:in? 

## NODE-Attribute

"99" steht für "keine Angabe"

id -> Identische ID wie aus der edgelist zur Identifikation der Knoten.

person -> Ganzer Name zusammengeschrieben z.B. SimonUnge 

type -> 0 = youtuber:in, 1 = Einnahmequellen (Bereiche wie z.B. Musik, Bücher, ...) und 2 = Organisationen (Management)

youtubechannel -> Name des Youtubekanals, Leerzeichen mit Unterstrich: Simon_Desue

youtubeabos -> Anzahl der Abonnenten auf Youtube in 1000er Schritten, also "25" für 25.000 Follower, "3.000" für 3 Mio

wealth -> Vermögen in Millionen Euro, also 1.5 für 1,5 Millionen Euro Vermögen

salary -> Einkommen pro Monat in 1000er-Schritten, also "25" für 25.000 Euro im Monat Verdienst mit Youtube

city -> In welcher Stadt lebt der:die Youtuber:in, Stadtname

age -> Alter des Youtubers

1 = 18 bis 22 Jahre 2 = 23 bis 27 Jahre 3 = 28 bis 32 Jahre 4 = über 32 Jahre

99 = jew. Contentbereich, nicht def. Alter

sex -> Geschlecht des Youtubers

1 = male, 2 = female, 3 = divers

country -> Landname, in dem Youtuber lebt.



