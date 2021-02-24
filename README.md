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

Begriffe:

Schlüssel (key) eines Relationenschemas R: K
ist ein Attribut, mit dessen Wert jede Zeile eindeutig identifiziert wird. Eine Schlüsselsuche auf Gleichheit wird immer maximal 1 Tabellenzeile als Ergebnis liefern.

Schlüsselkandidat
ist ein Attribut, mit dessen Wert jede Zeile eindeutig identifiziert werden könnte

Primärschlüssel
synonym für Schlüssel. Er identifiziert ein Objekt während seiner gesamten 'Lebensdauer'. Sein Wert kann nicht geändert werden, denn eine Änderung würde der Schaffung eines neuen Objektes gleichkommen.

Fremdschlüssel
ist ein Attribut, das in einer anderen Relation ein Primärschlüssel ist (foreign key)

Sekundärschlüssel
erlaubt den Zugriff auf ein oder mehrere Datensätze

Zusammengesetzter Schlüssel
Entitäten werden durch mehr als 1 Attribut identifiziert.

Arten von Primary Key:

Künstlicher Schlüssel (Surrogatschlüssel)
werden automatisch gebildet (z.B. als fortlaufende Nummer)

Natürlicher Schlüssel (sprechender Schlüssel)
ist ein Schlüsselkandidat mit einer Beziehung zu ein oder mehreren Attributen der Tabellenstruktur (z.B. die Kombination Vorname, Nachname, Geburtsdatum) oder ein Schlüsselkandidat, aus dem weitere Informationen abgelesen werden können  (z.B. ISBN Nummer, in die Land -, Verlags und Titelnummer codiert ist) )


