# Kessel-Temperatursteuerung + Abfüllstation

Zwei Sorgen, beide berechtigt, beide lösbar — und eine davon löst sich von selbst,
sobald man die Reihenfolge richtig herum denkt.

---

## Teil 1: „Der Kessel ist so träge" — das ist der Vorteil, nicht das Problem

### Die Physik in Zahlen

Dein Kessel hat ~110–125 L Nutzvolumen; real fährst du ihn mit **60–80 L Wasser**.
Spezifische Wärme Wasser = 4,19 kJ/(kg·K).

| Wassermenge | Wärmekapazität | 1 kWh extra = |
|---|---|---|
| 60 L | 251 kJ/K | **+14,3 K** |
| 70 L | 293 kJ/K | **+12,3 K** |
| 80 L | 335 kJ/K | **+10,8 K** |

**Heizrate bei 70 L Wasser:**

| Feuerleistung | Temperaturanstieg |
|---|---|
| 20 kW (volles Feuer) | 4,1 K/min |
| 15 kW | 3,1 K/min |
| 10 kW | 2,0 K/min |
| 5 kW (nur Glut) | **1,0 K/min** |
| 2 kW (Glut zusammengefallen) | 0,4 K/min |

Zum Vergleich aus [12](12_Kessel_Betrieb_Sicherheit.md): ein Holzfeuer in einem
Metzgerkessel bringt 10–20 kW, eine Herdplatte 2 kW.

**Energiebedarf für eine Ladung:** 70 L von 15 °C auf 80 °C = 19,1 MJ = **5,3 kWh**.
Bei 15 kW sind das **~21 Minuten Vollast.** Danach hält die Masse die Temperatur
fast allein.

---

### Warum „bei 70 °C Feuer aus → steigt auf 85 °C" keine Regel ist

Der Überschwinger ist **kein fester Wert**, sondern hängt davon ab, wie viel Glut
im Moment des Abdrehens noch Wärme nachschiebt:

| Restglut | Dauer bis Glut draußen | Überschwinger bei 70 L |
|---|---|---|
| 3 kW (schwach) | 3 min | **+1,8 K** |
| 5 kW (normale Glut) | 5 min | **+5,1 K** |
| 8 kW (volles Feuer, viel Glut) | 8 min | **+13,1 K** |

**→ Der Überschwinger ist proportional zur Heizrate im Moment des Abschaltens.**
Wer bei voller Flamme mit 4 K/min „Feuer aus" ruft, bekommt +10 bis +15 K.
Wer bei schwacher Glut mit 1 K/min abschaltet, bekommt +2 bis +3 K.

Gemini hat also **einen möglichen** Fall beschrieben, aber als Regel verkauft.
Dein Misstrauen war richtig.

**Die Konsequenz ist nicht „genauer zielen", sondern: langsam anfahren.**
Wer mit 1 K/min auf die Zieltemperatur zugeht, kann fast nicht überschießen.

---

### Das Protokoll (mit echten Zahlen für 70 L)

| Phase | Ziel | Feuer | Dauer | Steigrate |
|---|---|---|---|---|
| 1 | 15 → 60 °C | **volle Flamme**, Luft auf | ~15 min | 3 K/min |
| 2 | 60 → 72 °C | **keine Scheite mehr**, nur Glut | ~12 min | ~1 K/min |
| 3 | 72 → 77 °C | Glut an die Seite ziehen, Deckel drauf | ~5 min | 0,5 K/min |
| 4 | **bei 77 °C: Glut raus** in den Metalleimer | — | — | — |
| 5 | kriecht auf 79–81 °C | — | 2–3 min | — |
| 6 | **30 min halten** | 1 kleines Scheit alle 15–20 min | 30 min | ~0 |

**Die 30 min zählen ab dem Erreichen von 80 °C — nicht ab dem Anfeuern.**

**Warum in Phase 6 doch Holz nötig ist:** ein offener Kessel mit 70 L bei 80 °C
verliert grob 0,6–1,0 kW. Das sind **−0,12 bis −0,20 K/min**, also **−4 bis −6 K
über die 30 Minuten.** Start bei 81 °C, Ende bei 76 °C — passt.
Mit Deckel halbiert sich der Verlust.

---

### ⭐ Was du tun kannst, wenn er trotzdem drüber schießt

Das ist deine eigentliche Frage, und die Antwort ist: **eine ganze Menge.**
Du bist dem Feuer nicht ausgeliefert.

| # | Bremse | Wirkung | Wann |
|---|---|---|---|
| 1 | **Glut raus** mit der Schaufel in den Metalleimer | stoppt die Quelle | sofort |
| 2 | **Deckel ab** | Konvektion + Verdunstung, kühlt spürbar | ab ~85 °C |
| 3 | **Flaschen raus** mit dem Flaschenheber | rettet das, was wirklich gefährdet ist | ab ~90 °C |
| 4 | **Rühren / Wasser umwälzen** | verteilt Hot Spots, kühlt die Wand | immer |
| 5 | **Wasser nachgießen** | siehe unten | Notfall |

**Zu #5 — der einzige Punkt, der Fingerspitzengefühl braucht:**

| Zugabe in 70 L à 90 °C | Ergebnis |
|---|---|
| +10 L à 60 °C | 86,2 °C (−3,8 K) |
| +10 L à 20 °C | 81,2 °C (−8,8 K) |
| +20 L à 20 °C | 74,4 °C (−15,6 K) |

Kaltes Wasser wirkt also viermal so stark wie warmes — **aber** [12](12_Kessel_Betrieb_Sicherheit.md)
warnt zurecht vor Thermoschock auf der Emaille. Deshalb:
**immer erst Feuer runter, dann dünner Strahl seitlich an die Wand, nie in den
trockenen heißen Kessel.** Im Zweifel Flaschen raus statt Wasser rein — die Flaschen
sind das Wertvolle, das Wasser ist billig.

---

### Die eigentliche Beruhigung: dein Ziel ist ein Bereich, kein Punkt

Du hast im Kopf „80 °C exakt treffen, sonst verkocht der Saft". So funktioniert
Pasteurisation nicht.

**Pasteurisieren ist ein Produkt aus Temperatur × Zeit.** Maßgeblich ist, was im
**Kern der Flasche** ankommt — nicht was das Thermometer im Wasser anzeigt. Genau
deshalb dauert das Wasserbad 20–30 min, obwohl 80 °C für die Hefen eigentlich
schon nach Sekunden tödlich wäre: die Wärme muss erst durch Glas und Saft bis in
die Flaschenmitte. Wer zu kurz erhitzt, hat „am Flaschenrand heiß genug, im Zentrum
noch lebende Hefen" — und die Flasche gärt später.

**Daraus folgt die Umkehrung deiner Sorge:**

| Temperatur im Wasserbad | Bewertung |
|---|---|
| 75 °C | Minimum — funktioniert, aber knapp |
| **78–82 °C** | ⭐ **Zielbereich** |
| 85 °C | ✅ völlig ok, pasteurisiert schneller, minimal „gekochter" im Ton |
| 88–90 °C | ✅ Saft noch ok. ⚠️ **BVS-Alu-Verschluss max. 90 °C**, Kunststoffdeckel prüfen |
| 92–95 °C | ⚠️ deutlicher Kochgeschmack, Verschlüsse am Limit |
| ~100 °C | 🚨 **Sieden.** Offenes Wasserbad kommt über 100 °C gar nicht hinaus. Ab hier kann Saft in der Flasche zu kochen beginnen → Druck → Deckel fliegt oder Flasche platzt |

**Der Abstand zwischen deinem Ziel (80 °C) und dem echten Schadensfall (~100 °C)
ist 20 Kelvin — bei einer Masse, die sich mit 0,5 K/min bewegt. Das sind 40 Minuten
Reaktionszeit.**

Fachlich bestätigt: zwischen **80–90 °C und 1–30 min** Haltezeit sind die sensorischen
Unterschiede in der Praxis gering; entscheidend ist, dass die Pasteurisation
überhaupt wirkt. Mindestanforderung für Saft: **80 °C für ≥ 20 Sekunden**
([Fischer-Lahr](https://www.fischer-lahr.de/Konservieren-Einmachen)).

> **Dein Risiko ist nicht der Überschwinger. Dein Risiko ist der Unterschwinger:**
> zu kurz oder zu kalt → Hefe überlebt → Flaschenbomben im Vorratsregal.
> Lieber 84 °C und sicher als 78 °C und knapp.

### Ein Punkt, der in [12](12_Kessel_Betrieb_Sicherheit.md) fehlt: der Kopfraum

Saft dehnt sich beim Erhitzen aus — von 20 °C auf 80 °C um **+2,7 %**.

| Flasche | randvoll gefüllt bei 20 °C | Überdruck bei 80 °C |
|---|---|---|
| 0,7 L | 700 ml | **+19 ml** |
| 1,0 L | 1000 ml | **+27 ml** |

**Randvoll gefüllte Flaschen laufen im Wasserbad über oder drücken den Deckel hoch.**

→ **Fürs Wasserbad: 2–3 cm Kopfraum lassen.** Nicht randvoll.
(Bei reinem Hot Fill ist es umgekehrt — da füllt man randvoll, weil die Flasche
sofort verschlossen wird und beim Abkühlen Unterdruck entsteht.)

Beim Abkühlen entsteht dann das Vakuum, und bei MCA28 zieht sich der
Sicherheitsbutton nach innen — das ist dein **Dichtheits-Test.**

### Und: Abkühlen

Industriell wird aktiv gekühlt, weil langes Warmhalten das Aroma kostet.
**Für Glasflaschen gilt das nicht 1:1** — heiße Flaschen unter kaltes Wasser ist
Temperaturschock. Praxis für dich:

1. Feuer aus, Deckel drauf, **30–45 min im Wasser stehen lassen**
2. Flaschen raus, auf ein Holzbrett/Tuch (**nicht auf kalte Steinplatte**)
3. an einem zugfreien Ort auskühlen lassen, nicht stapeln

---

## Teil 2: Die Abfüllstation — deine Dampfentsafter-Idee

### Bewertung: die Idee ist gut, und zwar besser als du denkst

| Dein Punkt | Bewertung |
|---|---|
| Silikonschlauch + Klemme | ⭐ **Perfekt.** Dosierbar, absperrbar, spritzfrei |
| Flaschen im Getränkekasten unter dem Schlauch | ⭐ **Richtig.** Hände weg von der Hitze, Flaschen stehen sicher |
| Kesseldeckel zu lassen | ⭐ **Richtig.** 70 L mit Deckel verlieren fast nichts |
| Mehrere Flaschen pro Füllung des Oberteils | ✅ funktioniert |
| Saft bleibt auf Temperatur, weil Kessel Wärmespeicher | ✅ korrekt, aber siehe unten — **du brauchst die Temperatur gar nicht** |

### ⚠️ Vier Punkte zum Nachbessern

**1. Material.** Es muss das Oberteil des **Edelstahl**-Dampfentsafter sein, nicht
das Alu-Gerät aus dem Keller. Siehe [16](16_Dampfentsafter_eigenes_Produkt.md) —
Traubensaft pH ~3,5 löst Aluminium. Silikonschlauch ist ok (hält weit über 100 °C).

**2. Der kleine Behälter kühlt schnell aus.** 4–5 L Saft in einem offenen
Edelstahlgefäß verlieren deutlich schneller Wärme als 70 L im geschlossenen Kessel —
das Gefäß selbst schluckt beim ersten Mal einiges.
→ **Oberteil vorwärmen** (mit Heißwasser aus dem Kessel ausspülen), und den eigenen
Deckel drauf lassen.

**3. Hygiene.** Schlauch + Klemme **vorher auskochen.** Die Innenseite der Klemme
ist schlecht zu reinigen. Der Ausschöpf-Topf mit Henkel ist ein eigenes Werkzeug —
dediziert, ausgekocht, und der Henkel/der Rand darf niemals die Schlauchinnenseite
oder einen Flaschenhals berühren.

**4. Der Schlauch darf den Flaschenhals nicht berühren.** Knapp in die Mündung
halten, nicht reinstoßen. Sonst wandert Keim vom Hals in den Schlauch und von da
in die nächste Flasche.

### ⭐ Der Punkt, der deine ganze Sorge auflöst

Du schreibst: *„ich muss ja schauen, dass das zügig vonstatten geht, weil ich die
Hitze brauche, um die Deckel von innen zu entkeimen."*

**Das stimmt nur bei reinem Hot Fill. Bei deinem Plan stimmt es nicht.**

Dein Plan ist das **Wasserbad**: abfüllen → verschließen → **dann** 80 °C / 30 min.
In diesen 30 Minuten bekommt **die ganze Flasche inklusive Deckel, Dichtung und
Gewinde** 80 °C ab. Das ist eine **deutlich** zuverlässigere Deckelentkeimung als
zwei Minuten kopfüber mit heißem Saft.

**Daraus folgt:**

| | Hot Fill (Notlösung) | ⭐ Wasserbad (dein Plan) |
|---|---|---|
| Zeitdruck beim Füllen | **hoch** — Saft muss ≥80 °C haben beim Zuschrauben | **keiner** |
| Deckelentkeimung | durch heißen Saft, 2 min kopfüber | durch das Bad, 30 min |
| kopfüber stellen | ja (nur MCA28/PP28!) | **nein, entfällt** |
| Hantieren mit 80 °C heißem Saft | ja, über 50 Flaschen | **nein** |
| Weinflaschen (BVS) | ❌ nie kopfüber | ✅ stehend im Bad, kein Problem |
| Thermoschock an den Flaschen | Risiko | **keins** — alles erwärmt sich zusammen |
| Qualität | ok | ⭐ besser, 12+ Monate |

**Konkret heißt das: du kannst 50 Flaschen in aller Ruhe über eine Stunde füllen,
kalt, ohne Verbrennungsgefahr, ohne Stoppuhr.** Genau deshalb steht in
[01](01_Grundprinzip.md) der Satz „Reihenfolge umdrehen" — das war nie nur ein
Hygiene-Trick, das ist der Teil, der den Stress rausnimmt.

### Die Abfüllstation wird dadurch einfacher, nicht komplizierter

Weil du **nicht heiß** füllen musst, brauchst du den Kessel beim Füllen gar nicht:

```
   [SAMLA-Box / Behälter]              [KESSEL]
   Saft kalt oder angewärmt    →       Wasserbad
        ↓                              (läuft nebenher)
   Oberteil Dampfentsafter
   + Silikonschlauch + Klemme
        ↓
   Flasche im Getränkekasten
        ↓
   Deckel drauf, 2-3 cm Kopfraum
        ↓
   → in den Kessel, stehend, auf den Einlegerost
```

**Wichtig: Flaschen kommen in lauwarmes Wasser, nicht in heißes.** Kessel mit
Wasser füllen, Flaschen rein (Saft kalt = Flaschen kalt), **dann** anfeuern und
zusammen hochfahren. So gibt es keinen Temperaturschock, und das ist auch der
Standard beim Einkochen.

Wenn du die Aufheizzeit verkürzen willst: Saft vorher im Edelstahltopf auf dem
Gasring auf 40–50 °C anwärmen. Muss aber nicht.

### Reihenfolge der Chargen

1. **Erst die angegorene Charge** — die hat keinen Puffer mehr
2. Dann die frische
3. **Zweite Ladung:** das heiße Wasser im Kessel lassen, Flaschen tauschen,
   nur kurz nachheizen. Spart ~15 min und die Hälfte des Holzes.

---

## Checkliste für heute abend

- [ ] Zwei Thermometer, beide **im Wasser**, verschiedene Stellen
- [ ] Metalleimer + Schaufel für die Glut griffbereit
- [ ] Einlegerost im Kessel
- [ ] Wasserstand über Flaschenschulter
- [ ] **Flaschen mit 2–3 cm Kopfraum** füllen
- [ ] Phase 2 einhalten: ab 60 °C **keine Scheite mehr nachlegen**
- [ ] Bei 77 °C Glut raus
- [ ] **Timer stellen ab 80 °C** — 30 min
- [ ] 1 kleines Scheit alle 15–20 min in der Haltephase
- [ ] Feuer aus → 30–45 min stehen lassen → Flaschen auf Holz/Tuch, nicht auf Stein
- [ ] Nach 24 h: **Deckel-Test.** MCA28-Button eingezogen = dicht.
  Jeder Deckel, der sich hochdrücken lässt → Flasche sofort in den Kühlschrank, zuerst trinken
