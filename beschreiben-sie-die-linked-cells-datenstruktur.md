# Note
```
guid: Fqavvi>m3D
notetype: Einfach
```

### Tags
```
```

## Vorderseite
Beschreiben sie die Linked-Cells Datenstruktur

## Rückseite
Der Zweck ist die Auffindung von benachbarten Partikeln unter der
Betrachtung von O(1) anderer Partikel.
<ul>
  <li>Das Simulationsgebiet wird dazu mit Hilfe eines regulären
  Gitters in kleine Zellen eingeteilt, das Gitter hat dann n Zeilen
  und m Spalten. Im einfachsten Fall sind die Zellen quadratisch
  und die Kantenlänge entspricht exakt dem Abschneideradius.
  <li>Gespeichert werden die Zellen in einem fortlaufenden Array,
  in dem die Zeilen hintereinander folgen
  <li>Die Partikel werden in jedem Zeitschritt über ihre
  aktuellePosition in die jeweiligen Zellen einsortiert, danach
  werden alle Zellen durchlaufen, wobei für jeden Partikel nur mehr
  die 8 direkt umliegenden Zellen zur Auffindung benachbarter
  Partikel und zu Berechnung betrachtet werden müssen
  <li>Eine Randschicht rund um das Simulationsgebiet mit den
  jeweils gegenüberliegenden Randzellen ermöglicht, dass alle
  Zellen 8 benachbarte Zellen für die Betrachtung haben
  <li>Dank des dritten Newton'schen Gesetzes muss jedes Paar von
  Partikeln nur einmal betrachtet werden, womit wir nur mehr Zellen
  mit höherem Index betrachten müssen und nicht mehr alle 8
</ul>
