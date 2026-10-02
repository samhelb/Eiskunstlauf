# Datensatz Eiskunstlauf

Codebuch Stand 2026-10 erstellt von Sam Helbling

## EDGE-Attribute

**from** entspricht ID (Kürzel). definiert den Sender in gerichteten
Netzwerken. Entspricht ID in der Nodelist. Keine Sonderzeichen, etc.

**to** entspricht ID (Kürzel). definiert den Empfänger in gerichteten
Netzwerken. Entspricht ID in der Nodelist. Keine Sonderzeichen, etc

**realtionship** definiert die Art der Beziehung: 1=Skater/Trainer
2=Skater/Land 3=Trainer/Land 4=Skater/Championship

**winstogether** Menge an Betreuungen (z.B. 4 Wettkämpfe zusammen - Wert
4). Ausprägung der Kantenstärke (Beziehungsstärke), definiert nach
vorgegeben Skalen.

## NODE-Attribute

**id** Identische ID wie aus der edgelist zur Identifikation der Knoten.
In diesem Fall entsprechen die IDs dem Kürzel des vollen Namens. Bei
Doppelungen werden die letzten Zwei Ziffern des Geburtsjahrs angehängt
(z.B. ah01).

**name_long** Ganz ausgeschriebener Name für Vollständigkeit in der
Tabelle

**name_short** nur Nachname, für übersichtlichere Visualiserung; Bei
Doppelung wird der erste Buchstaben des Vornamens angefügt (z.B. "NSato"
statt "Sato")

**sex** 1 = weiblich 2 = männlich 3 = divers

**points** Jede Platzierung in den Top 5 liefert in unserem System
Punkte: Platz 1 = 5 Punkte Platz 2 = 4 Punkte Platz 3 = 3 Punkte Platz 4
= 2 Punkte Platz 5 = 1 Punkt Die Punkte werden über Wettkämpfe hinweg
addiert. Zeigt die "Macht" der Skater\*innen.

**type** relevant bei two-mode Netzwerken, um die Unterscheidung
zwischen z.B. Akteur und Event zu berechnen: 0 = Skater 1 = Trainer 2 =
Nationalität 3 = Championship
