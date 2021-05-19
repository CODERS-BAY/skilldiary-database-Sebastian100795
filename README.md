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

BEZIEHUNGEN
ternär
  Drei beteiligte Entitäten
unär
  Eine beteiligte Entität
 Am häufigsten: binär
  Zwei beteiligte Entitäten
Eine Beziehung verbindet (assoziiert) wechselseitig zwei Entitäten

DBMS TYpen
Folgende wesentliche Datenbanktypen können unterschieden werden:
Hierarchische DBMSs
Netzwerkartige DBMSs
Relationale DBMSs
Invertierte Listen DBMSs
Objektrelationale DBMS
Objektorientierte DBMS

Wozu das Ganze???
Strukturierung der Datenmengen
Niemand kennt im Unternehmen ‚alle Daten‘
Optimierung der vorhandenen Daten

Daten sind im strategischen Interesse eines Unternehmens
Integration in den Gegenstand 'Systemplanung und Projektentwicklung'

Komponenten eines DBMS

Datenbankmanagementsystem
Data Dictionary
Logdateien
Datendateien
verschiedene Puffer 
Endbenutzerschnittstellen

Funktionen eines DBMS
Insert, update und delete von Daten
Verwaltung von Metadaten
Vorkehrungen zu Datensicherheit und Datenschutz
Vorkehrungen zur Datenintegrität
Ermöglichung eines Mehrbenutzerbetriebs (Transaktionen)
Bereitstellung von Kennzahlen über Betrieb des DBMS

Einige Vorteile einer DB

Verminderung der Redundanz - schnellere Aktualisierung der Daten.
Einhaltung der Datenintegrität: die Zentralisierung der Kontrolle erlaubt eine  einfachere Überprüfung der Daten auf
Korrektheit und Vollständigkeit  (Datenkonsistenz).
Irrtümliche, absichtliche oder durch Fehler hervorgerufene Verfälschung von Daten
Verfälschungen von Daten können durch gelegentlich auszuführende Prüfprogramme einfacher entdeckt werden.
Verbesserter Schutz der Daten vor unberechtigtem Zugriff durch die einheitliche Kontrolle beim Zugang zur Datenbasis.
Datenunabhängigkeit: die Änderung der physikalischen Organisation der Daten erfordert keine Änderung der  Anwendungsprogramme.
spezifische Datensicht: der Benutzer sieht nach Form und Menge nur die ihn betreffenden Daten.

Synonyme
unterschiedliche Bezeichnungen für eine Entität, die logisch dieselbe Entität kennzeichnet.

Zustellung
                  = Versand
Auslieferung

Homonyme
ein Name wurde vergeben, jedoch sind unterschiedliche logische Entitäten gemeint.
   
                Kundenbestellung
Bestellung  =
                Lieferantenbestellung

Arten von Primary Key

Künstlicher Schlüssel (Surrogatschlüssel)
werden automatisch gebildet (z.B. als fortlaufende Nummer)

Natürlicher Schlüssel (sprechender Schlüssel)
ist ein Schlüsselkandidat mit einer Beziehung zu ein oder mehreren Attributen der Tabellenstruktur (z.B. die Kombination Vorname, Nachname, Geburtsdatum) oder ein Schlüsselkandidat, aus dem weitere Informationen abgelesen werden können  (z.B. ISBN Nummer, in die Land -, Verlags und Titelnummer codiert ist) )

Sub- Supertyp

Synonym: Generalisierung / Spezialisierung
Synonym: 'is-a' Beziehung

Bei der Spezialisierung wird ein Entitätstyp als Teilmenge eines anderen, ‚übergeordneten‘ Entitätstyps angenommen. Im Supertyp sind alle Attribute, die den Subtypen gemeinsam sind. Im Subtyp 1 findet man alle Attribute, die nur dort und nicht in den anderen Subtypen oder dem Supertyp vorkommen. Damit generalisiert der Supertyp.

Redundanz
Redundanz ist die mehrmalige Speicherung ein und derselben Information

Anomalie
Update Anomalie
ändert sich die Studentenadresse, so sind alle davon betroffenen Datensätze zu ändern

Insert Anomalie
es wird ein neuer Student aufgenommen, der derzeit keine Vorlesung besucht. Da der Schlüssel vollständig angegeben werden muss, ist es nicht möglich auf den Schlüsselteil Vorlesungsnummer zu verzichten.

Delete Anomalie
wird der letzte Student einer Vorlesung gelöscht, so ist der Name der Vorlesung nicht mehr bekannt.
Normalform
1NF: funktional abhängig vom Gesamtschlüssel
2NF: keine funktionalen Abhängigkeiten von Schlüsselteilen
3NF: keine funktionalen Abhängigkeiten von Nichtschlüsselattributen





Arten von Primary Key:

Künstlicher Schlüssel (Surrogatschlüssel)
werden automatisch gebildet (z.B. als fortlaufende Nummer)

Natürlicher Schlüssel (sprechender Schlüssel)
ist ein Schlüsselkandidat mit einer Beziehung zu ein oder mehreren Attributen der Tabellenstruktur (z.B. die Kombination Vorname, Nachname, Geburtsdatum) oder ein Schlüsselkandidat, aus dem weitere Informationen abgelesen werden können  (z.B. ISBN Nummer, in die Land -, Verlags und Titelnummer codiert ist) )


