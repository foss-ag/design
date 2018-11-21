Bei Druckdaten ist zu beachten, dass es sowohl den Beschnitt (bleed) als auch den Sicherheitsabstand (margin) gibt.

Der Beschnitt wird außen an das Produktformat angefügt.
Ein runder Sticker mit 70mm Größe bei 3mm auf allen Seiten hat also im Datenformat 76mm,
wovon an jeder Seite 3mm abgeschnitten werden.
Da die Druckereien aber nicht gewährleisten können, dass immer exkat gearbeitet wird,
empfielt es sich alle Hintergründe bis an den Rand des Datenformats zu legen, sodass keine weißen Ränder enstehen.

Der Sicherheitsabstand ist die der Abstand den alle wichtigen Bildelemente einhalten sollten,
damit sie auch bei Ungenauigkeiten in der Fertigung nicht abgeschnitten werden.
Dieser wiederum ist Teil des Produktformats und ist auch auf dem Endprodukt zu sehen.
Bei einem runden 70mm Sticker bedeutet das,
dass bei 4mm Sicherheitsabstand die Bildelemente eine größe von maximal 62mm im Durchmesser haben sollten.

Bei den Druckdateien in den Repos der FOSS-AG hat sich das folgende Namensschema für die Druckdaten etabliert:

<Druckprodukt>-<Name>_<Größe>+<Beschnitt>.<dateityp>
