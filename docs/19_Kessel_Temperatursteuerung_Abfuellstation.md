# Kessel-Temperatursteuerung + Abfüllstation

Zwei Sorgen, beide berechtigt. Die eine löst sich durch Rechnen, die andere durch
einen Trick, den du noch nicht auf dem Zettel hast.

> **Verfahren, um das es hier geht:** Saft komplett in der emaillierten Einlage des
> Schlachtkessels erhitzen → **heiß abfüllen (Hot Fill)** → 2–3 min kopfüber.
> Nicht das Wasserbad-Verfahren. Begründung in
> [07_Schlachtkessel.md](07_Schlachtkessel.md), Abschnitt „Entscheidung Modus B".

---

## Teil 1: „Der Kessel ist so träge" — das ist der Vorteil, nicht das Problem

### Die Physik in Zahlen

Dein Kessel hat ~110–125 L Nutzvolumen, Innendurchmesser ~59 cm. Für ~50 L Saft
ergibt das eine **Füllhöhe von nur 18 cm** — der Rest ist Freibord (gut so, dazu unten mehr).

Spezifische Wärme Wasser/Saft ≈ 4,19 kJ/(kg·K).

| Inhalt | Wärmekapazität | 1 kWh extra = |
|---|---|---|
| 50 L Saft | 209 kJ/K | +17,2 K |
| 70 L Wasser | 293 kJ/K | +12,3 K |
| 80 L Wasser | 335 kJ/K | +10,8 K |

**Heizrate bei 50 L Inhalt:**

| Feuerleistung | Temperaturanstieg |
|---|---|
| 20 kW (volles Feuer) | 5,7 K/min |
| 15 kW | 4,3 K/min |
| 10 kW | 2,9 K/min |
| 5 kW (nur Glut) | **1,4 K/min** |
| 2 kW (Glut zusammengefallen) | 0,6 K/min |

Ein Holzfeuer bringt 10–20 kW, eine Herdplatte 2 kW ([12](12_Kessel_Betrieb_Sicherheit.md)).

**Energiebedarf:** 50 L Saft von 15 °C auf 85 °C = 14,7 MJ = **4,1 kWh** → bei 15 kW
**~16 Minuten Vollast.** Danach hält die Masse die Temperatur fast allein.
Ohne Feuer und mit Deckel verliert sie nur **−0,23 bis −0,34 K/min**.

---

### Warum „bei 70 °C Feuer aus → steigt auf 85 °C" keine Regel ist

Der Überschwinger hängt davon ab, wie viel Glut im Moment des Abdrehens noch nachschiebt:

| Restglut | Zeit bis Glut draußen | Überschwinger bei 50 L |
|---|---|---|
| 3 kW (schwach) | 3 min | **+2,6 K** |
| 5 kW (normale Glut) | 5 min | **+7,2 K** |
| 8 kW (volles Feuer, viel Glut) | 8 min | **+18,4 K** |

**→ Der Überschwinger ist proportional zur Heizrate im Moment des Abschaltens.**
Wer bei voller Flamme mit 5,7 K/min „Feuer aus" ruft, landet bei +15 bis +18 K.
Wer bei schwacher Glut mit 1,4 K/min abschaltet, bekommt +3 bis +5 K.

Die „70 °C anheizen, er steigt auf 85" ist also **ein möglicher** Fall, keine Regel.
**Die Lösung ist nicht genauer zielen, sondern langsam anfahren.**

### ⚠️ Bei Hot Fill ist der Überschwinger ernster zu nehmen als beim Wasserbad

Das ist der Unterschied, den du richtig gespürt hast:

| | Wasserbad (Modus A) | ⭐ **Hot Fill (dein Verfahren)** |
|---|---|---|
| Was wird heiß | Wasser | **der Saft selbst** |
| 90 °C | Saft merkt es kaum (Flaschenkern kühler) | ⚠️ **direkt im Saft** → Kochgeschmack |
| Obergrenze | ~100 °C (Sieden) | **90 °C** — „sonst Kochgeschmack und Aromaverlust" ([06](06_Einkochtopf.md)) |
| Ab 95 °C | Glas-/Verschlussproblem | **Aroma kaputt, nicht reparabel** |

**Dein Zielband ist also 82–86 °C, hartes Limit 90 °C.** Das ist enger als beim
Wasserbad — aber mit ~24 cm Freibord und 1,4 K/min bei reiner Glut gut zu fahren.

### Das Protokoll (für ~50 L Saft)

| Phase | Ziel | Feuer | Dauer | Steigrate |
|---|---|---|---|---|
| 1 | 15 → 60 °C | volle Flamme, **rühren** | ~12 min | 4–5 K/min |
| 2 | 60 → 75 °C | **keine Scheite mehr**, nur Glut | ~11 min | ~1,4 K/min |
| 3 | 75 → 80 °C | Glut an die Seite, Deckel drauf | ~4 min | ~0,6 K/min |
| 4 | **bei 80 °C: Glut raus** in den Metalleimer | — | — | — |
| 5 | kriecht auf 83–86 °C | — | 2–3 min | — |
| 6 | abfüllen | Glut nach Bedarf zurück | ~45–60 min | ~0 |

**Der Timer läuft nicht mit.** Du hast ab Phase 5 beliebig Zeit zum Abfüllen, weil
50 L mit Deckel nur ~0,3 K/min verlieren — und du bei Bedarf ein Scheit nachlegst.

---

### ⭐ Die fünf Bremsen, wenn er trotzdem drüber schießt

Du bist dem Feuer nicht ausgeliefert:

| # | Bremse | Wirkung |
|---|---|---|
| 1 | **Glut raus** mit Schaufel + Metalleimer | stoppt die Quelle sofort |
| 2 | ⭐ **kalten Saft aus dem nächsten Behälter nachgießen** | **die beste Bremse — siehe unten** |
| 3 | **Deckel ab** | Konvektion + Verdunstung |
| 4 | **rühren** | verteilt Hot Spots, kühlt die Wand |
| 5 | Feuer ganz raus, Kessel von der Glut ziehen (Rollen!) | ultima ratio |

**Zu #2 — der Trick, den du beim Wasserbad nicht hast:**

Beim Wasserbad müsstest du Wasser nachgießen und riskierst Thermoschock auf der Emaille.
Bei Hot Fill ist die „Kühlflüssigkeit" **dein eigener Saft**:

| Zugabe in 45 L à 90 °C | Ergebnis |
|---|---|
| +5 L à 15 °C | **82,5 °C** (−7,5 K) |
| +10 L à 15 °C | **76,3 °C** (−13,7 K) |

**Kein Thermoschock** (du gießt Flüssigkeit in Flüssigkeit, nicht auf trockene heiße
Emaille), **keine Verdünnung** (es ist derselbe Saft), und die Charge wird einfach größer.

→ **Praktische Konsequenz: stell dir immer einen Behälter kalten Saft griffbereit
neben den Kessel.** Das ist dein Notausgang, und er kostet nichts.

---

### Was bei welcher Temperatur wirklich passiert (Hot Fill)

| Safttemperatur | Bewertung |
|---|---|
| < 78 °C | ❌ **zu kalt zum Abfüllen** — Deckel-/Halsentkeimung wirkt nicht sicher |
| **82–86 °C** | ⭐ **Zielbereich** |
| 88–90 °C | ⚠️ Obergrenze. Noch ok, aber nicht länger |
| > 90 °C | ❌ Kochgeschmack, Aromaverlust — **nicht reparabel** |
| ~100 °C | 🚨 Sieden, Schaum über, Verlust |

> **Anders als beim Wasserbad ist hier der Überschwinger das größere Risiko,
> nicht der Unterschwinger.** Aber beides ist mit „langsam anfahren + kalter Saft
> als Bremse" sicher im Griff.

### ⚠️ Füllmenge: Hot Fill = **randvoll**

Das ist das **Gegenteil** vom Wasserbad. Beim Wasserbad brauchst du 2–3 cm Kopfraum,
weil sich der Saft ausdehnt. Bei Hot Fill willst du **möglichst wenig Luft**, denn
beim Abkühlen zieht sich der Saft zusammen und erzeugt das Vakuum:

| Flasche | randvoll bei 85 °C gefüllt | Vakuum/Kopfraum bei 20 °C |
|---|---|---|
| 0,5 L | 500 ml | 14 ml |
| 0,7 L | 700 ml | 19 ml |
| 1,0 L | 1000 ml | 27 ml |

**Randvoll füllen, sofort verschließen.** Nach 24 h ist der MCA28-Sicherheitsbutton
eingezogen — das ist dein **Dichtheitstest**.

### ⚠️ Freibord: der angegorene Saft schäumt

CO₂ geht beim Erhitzen schlagartig raus. Bei 50 L Saft = 18 cm Füllhöhe in einem
40–45 cm tiefen Kessel hast du **~24 cm Freibord** — das reicht. Aber:
- **Schaum abschöpfen**, solange er kommt (er trägt Hefe und Trub)
- nie bis oben füllen
- Phase 1 nicht mit voller Flamme durchprügeln, sonst kocht es über ins Feuer

---

## Teil 2: Deine Abfüllstation — die Idee ist gut

### Bewertung

| Dein Punkt | Bewertung |
|---|---|
| Silikonschlauch + Klemme | ⭐ **Perfekt.** Dosierbar, absperrbar, spritzfrei |
| Flaschen im Getränkekasten unterm Schlauch | ⭐ **Richtig.** Hände weg von der Hitze, Flaschen stehen sicher |
| Kesseldeckel zu lassen | ⭐ **Richtig.** 50 L verlieren mit Deckel nur ~0,3 K/min |
| Mit Topf + Henkel ausschöpfen und nachfüllen | ✅ funktioniert |
| Kessel muss nicht ständig geöffnet werden | ✅ korrekt |

### Nachbessern — drei Punkte

1. **Nur das Edelstahl-Oberteil**, nicht das Alu-Gerät ([16](16_Dampfentsafter_eigenes_Produkt.md))
2. **Oberteil vorwärmen** — ein kaltes 1,2-kg-Edelstahlgefäß schluckt beim ersten
   Füllen **2,1 K** aus den 4,5 L Saft. Einmal mit Heißwasser ausspülen, weg ist es.
3. **Schlauch + Klemme vorher auskochen.** Die Innenseite der Klemme ist der
   schwierigste Punkt.

### 😅 Rücknahme: „Der Stutzen darf den Flaschenhals nicht berühren"

**Das war übertrieben und unpraktisch — vergiss es.** Du hattest recht, das ist
nicht sauber hinzubekommen, und ein Trichter wäre schlimmer (mehr Fläche, wird kalt,
berührt den Hals genauso).

Der Schlauch wird **dauernd mit 82–86 °C heißem Saft durchspült** — er entkeimt sich
dabei selbst. Was tatsächlich zählt:

- ✅ **Der Schlauch darf in der Flaschenmündung aufliegen.** Völlig ok.
- ❌ Er darf **nichts anderes** berühren: Tisch, Boden, deine Hände, Flaschenaußenseiten
- ❌ Nicht zwischendurch ablegen. Wenn doch: kurz in heißes Wasser
- ❌ Kein Desinfektionsspray (siehe [20](20_Einkauf_heute.md))

Es gibt dafür übrigens ein Fertigteil: ein **Abfüllröhrchen mit Federhahn** aus dem
Brau-/Weinbedarf (~5 €). Das wird in den Flaschenhals gedrückt, steht von selbst und
stoppt den Fluss beim Anheben. Genau für diesen Zweck gebaut. Kein Muss — deine
Klemme tut es auch.

---

## ⭐ Teil 3: Die Hektik — gerechnet statt befürchtet

Deine Sorge: *„ich muss schauen, dass das zügig vonstatten geht, weil ich die Hitze
brauche, um die Deckel von innen zu entkeimen."*

### Das Zeitfenster ist ~10 Minuten, nicht 30 Sekunden

Dein Umfüllgefäß (Dampfentsafter-Oberteil, ~4,5 L) hat eine Wärmekapazität von
**18,9 kJ/K**. Geschätzter Wärmeverlust eines offenen 4,5-l-Edelstahlgefäßes bei
85 °C in 15 °C Umgebung: 80–200 W.

| Verlust | Abkühlrate | Zeit von 85 auf 80 °C |
|---|---|---|
| 80 W | −0,25 K/min | **20 min** |
| 150 W | −0,48 K/min | **10 min** |
| 200 W | −0,64 K/min | **8 min** |

**4,5 L sind ~6 Flaschen à 0,7 L.** Also selbst im schlechtesten Fall **über eine
Minute pro Flasche.** Das ist kein Sprint.

### Und es gibt gar keine irreversible Uhr

Der Kessel hält 50 L bei 83–86 °C praktisch beliebig lange (Deckel zu, gelegentlich
ein Scheit). **Das Umfüllgefäß ist nur ein Puffer.** Wenn es abkühlt: Saft zurück
in den Kessel oder frischen heißen nachschöpfen. **Nichts geht verloren, nichts
muss in einer bestimmten Zeit fertig sein.**

### ⭐ Der eigentliche Trick: entkoppele die Deckelentkeimung vom Tempo

Dein Flaschenhals wird durch den heißen Saft entkeimt — **der Deckel muss das nicht
über den Saft machen.** Mach ihn vorher keimfrei, dann ist es völlig egal, wie
schnell du arbeitest:

1. **Alle Deckel 5 min in kochendem Wasser** (zweiter Kessel oder großer Topf)
2. **im heißen Wasser liegen lassen**
3. mit einer **ausgekochten Zange** greifen, aufschrauben
4. **fertig.** Kein Wettlauf.

Damit bleibt das Kopfüberstellen eine **zusätzliche** Sicherheit, nicht die einzige.

### Kopfüber — so geht es ohne Akrobatik

- **Nur bei MCA28 / PP28 / PP31,5.** 🚨 **BVS-Weinflaschen niemals kopfüber** —
  nur stehend, siehe [08](08_Gewindenormen_Referenz.md)
- **Im Getränkekasten:** Flaschen kopfüber in den Kasten stellen, Kasten auf ein
  Brett. Damit kannst du 12–20 Stück auf einmal stellen, statt sie in der Hand zu halten
- **2–3 Minuten reichen**, dann umdrehen und stehend auskühlen
- Nicht stapeln, nicht auf kalte Steinplatte

### Abkühlen

Industriell wird aktiv gekühlt, weil langes Warmhalten das Aroma kostet
([Fischer-Lahr](https://www.fischer-lahr.de/Konservieren-Einmachen)). **Heiße Glasflaschen
unter kaltes Wasser ist aber Temperaturschock.** Praxis für dich:

1. nach dem Kopfüberstellen **aufrecht, zugfrei** auskühlen lassen
2. nicht stapeln (Wärmestau)
3. nicht auf kalte Steinplatte — Holzbrett oder Handtuch
4. **nach 24 h Dichtheitstest:** Button eingezogen? Deckel fest? nichts ausgelaufen?
   Jede Flasche, die durchfällt → sofort in den Kühlschrank, zuerst trinken

---

## 🚨 Der Punkt, der bei Hot Fill wirklich kritisch ist: Anbrennen

Das ist das eigentliche Risiko von Modus B, nicht die Temperatur.

**Holzfeuer direkt unter der Emaille + Saft mit Trub und Hefesatz am Boden = der Satz
brennt an.** Angebrannter Hefesatz gibt einen bitter-röstigen Ton an die ganze Charge ab,
und du bekommst ihn nicht mehr raus. Bei 18 cm Füllhöhe liegt der Satz direkt über der
Flamme.

**Deshalb, in dieser Reihenfolge:**

1. **Saft kalt stehen lassen**, bis sich der Trub abgesetzt hat (hast du schon)
2. **Klaren Saft abziehen** — genau dafür brauchst du den Schlauch
   (8–12 mm, siehe [20](20_Einkauf_heute.md))
3. **Bodensatz separat** in einen Topf → später durch ein Tuch pressen oder verwerfen
4. **Erst dann in den Kessel**
5. **Phase 1 rühren**, bis ~50 °C — danach ist Konvektion genug
6. **Nicht mit voller Flamme durchheizen**, wenn der Saft schon warm ist

### Alternative, falls dir das Feuer zu unkontrollierbar ist

Du hast einen **Gaskocher-Ring** und einen **~28-l-Edelstahltopf** ([09](09_Bestandsaufnahme_Fotos.md)).

| | Kessel (Holz) | Gasring + 28-l-Topf |
|---|---|---|
| Menge pro Charge | 50 L am Stück | 2 × ~22 L |
| Regelbarkeit | ⚠️ träge | ⭐ **stufenlos** |
| Anbrennen | ⚠️ Risiko | ✅ gering |
| Aufwand | 1 × anfeuern | 2 × erhitzen |
| Kessel-Rolle | Saft erhitzen | ⭐ **Heißwasser**: Flaschen vorwärmen, Deckel auskochen, reinigen |

**Der Gasring ist der kontrollierbarere Erhitzer, der Kessel das bessere Logistikzentrum.**
Wenn du dich mit dem Feuer unwohl fühlst: Saft auf dem Gasring, Kessel für Heißwasser.
Beide Wege führen zum selben Produkt.

---

## Checkliste für heute abend

- [ ] **Saft abziehen** — klarer Saft in den Kessel, Bodensatz separat
- [ ] **Einen Behälter kalten Saft als Notbremse** neben den Kessel stellen
- [ ] Zwei Thermometer, **im Saft**, verschiedene Stellen
- [ ] **Alle Deckel 5 min auskochen** und im heißen Wasser liegen lassen
- [ ] Ausgekochte Zange für die Deckel bereitlegen
- [ ] Oberteil + Schlauch + Klemme auskochen, Oberteil vorwärmen
- [ ] Metalleimer + Schaufel für die Glut
- [ ] Ab 60 °C **keine Scheite mehr**, bei 80 °C **Glut raus**
- [ ] **Schaum abschöpfen**, Freibord im Auge behalten
- [ ] Ziel **83–86 °C**, hartes Limit **90 °C**
- [ ] **Randvoll** füllen, sofort verschließen
- [ ] **2–3 min kopfüber** im Kasten — **außer BVS-Weinflaschen**
- [ ] aufrecht, zugfrei auskühlen, nicht stapeln
- [ ] **nach 24 h Dichtheitstest**
