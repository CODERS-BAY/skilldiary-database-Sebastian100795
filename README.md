Tag 2

Arten von Datenbanken 

Hierarchische DBMSs
Netzwerkartige DBMSs
Relationale DBMSs
Invertierte Listen DBMSs
Objektrelationale DBMS
Objektorientierte DBMS

Hierachische DB:

Man erhält also eine Menge von Dateien (bzw. Listen), die untereinander hierarchisch in Beziehung stehen. Daher orientieren sich hierarchische DBMS an der Implementierung von 1:n-Relationships. 

Netzwerkartige DBMSs:

Die Informationsstruktur wird mit Hilfe von Netzwerken dargestellt. Anders als bei hierarchischen Systemen existieren keine Wurzelobjekte.

Relationale DBMSs:

Alle Informationen in einer relationalen Datenbank werden explizit und in eindeutiger Weise auf der logischen Ebene dargestellt. Dies geschieht durch Tabellen.

Tag 3

Normalisierung:

1NF
Eine in 1. Normalform befindliche Relation enthält keine Attribute, die sich aus mehreren Elementen zusammensetzen.
In einer 1NF Relation ist im Kreuzungspunkt einer Kolonne (Spalte, Attribut) und einer Reihe (Zeile, Tupel) jederzeit nur 1 Wert vorzufinden.
Eine in 1.Normalform befindliche Relation R(S,A,B,C) mit Primärschlüssel S ist dadurch gekennzeichnet, daß A, B und C von S funktional abhängig sind vom Gesamtschlüssel (d.h. es sind keine Wiederholfelder erlaubt).

2NF

Eine in 2.Normalform befindliche Relation ist dadurch gekennzeichnet, daß jedes nicht dem Schlüssel angehörende Attribut funktional abhängig ist vom Gesamtschlüssel (=1.NF) nicht aber von den einzelnen Schlüsselteilen.
Eine Relation ist in 2NF, wenn sie in 1NF ist und jedes nicht dem Schlüssel angehörende Attribut voll funktional abhängig ist vom Gesamtschlüssel.

3NF

Eine in 3.Normalform befindliche Relation ist dadurch gekennzeichnet, dass jedes nicht dem Schlüssel angehörende Attribut funktional abhängig ist vom Gesamtschlüssel (=1.NF), nicht aber von einzelnen Schlüsselteilen (=2.NF). Weiters sind keine transitiven Abhängigkeiten (funktionale Abhängigkeiten zwischen Nicht-Schlüssel-Attributen) erlaubt.
Eine Relation ist in 3NF, wenn sie in 2NF ist und keine transitiven Abhängigkeiten aufweist.

