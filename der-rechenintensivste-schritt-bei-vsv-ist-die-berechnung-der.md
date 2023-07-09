# Note
```
guid: fq9(Pp?;&n
notetype: Einfach
```

### Tags
```
```

## Vorderseite
Der rechenintensivste Schritt bei VSV ist die Berechnung der Kräfte / Beschleunigung mit O(N²). Wie kann man hier optimieren?

## Rückseite
<ul>
  <li>Erklärung des Abschneideradius: Wenn eine Kraft mit
  Vergrößerung des Abstands zu ihr sehr schnell nachlässt genügt es
  nur Partikel mit sehr kleinem Abstand zu betrachten. Den Abstand
  ab dem diese berücksichtigt werden, nennt man Abschneideradius.
  Die Anzahl der Partikel, die sich innerhalb dieses Radius
  befinden ist durch eine Konstante begrenzt, daher lässt sich die
  Kraft auf einen Partikel mit O(1) Operationen berechnen und damit
  die Kräfte auf alle Partikel mit O(N) Operationen.
  <li>Dieser ist bei der Gravitation höher zu wählen als bei
  Molekülen, weil die Gravitation nur quadratisch und damit
  langsamer als bei Molekülen nachlässt
</ul>
