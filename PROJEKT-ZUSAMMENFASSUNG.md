# Cognizance World — Projekt-Übergabe & Zusammenfassung

> **Eine Datei für alles.** Dieses Dokument ist die *einzige* aktuelle Projekt-Übersicht.
> Es ersetzt jede vorherige Fassung. In einen anderen Claude-Chat oder als Wissensquelle
> ins claude.ai-Projekt hochladen. **Immer nur die neueste Version im Projekt behalten.**
> **Stand: 15. Juli 2026 — Video-Startseite LIVE; Portal-Zeremonie auf „UFO-Einflug" umgebaut.**

---

## 0. Das Wichtigste zuerst (aktueller Stand)

**Die neue interaktive Video-Startseite ist fertig, integriert und LIVE** auf `cognizance-website.pages.dev`.
Sie hat das alte WebGL-Schwarze-Loch-Intro **komplett ersetzt**. Die ganze Kette läuft:

> **Video 1 (blaues Quanten-Netz, Ambient-Schleife) mit Gravitationslinse** → **„ERKENNE" gedrückt halten**
> (goldener Lade-Ring) → **Lichtblitz (Naht 1)** → **Video 2 (der Flug)** → **ab Sek. 9 abdunkeln auf `#080815` (Naht 2)**
> → **Portal-Menü**, ceremoniell aufgebaut (Schriftzug „Cognizance World" Buchstabe für Buchstabe, dann die 4 Tore
> nacheinander, dann die Ziffern) → **voll klickbar** (Kapitel I, Platzhalter II–IV, Navigation).

**Nächste offene Ziele:** Inhalte für Portale II & IV, Portal III (Holodeck, Abschnitt 6), Sound für Video 2,
Feinschliff der Timings, Domain-Entscheidung. Details in Abschnitt 8.

---

## 1. Was ist das Projekt?

Ein interaktives digitales **Kunstwerk über Wahrnehmung, Quantenphysik und Bewusstsein**.
Eine einzelne, statische Website, live über **Cloudflare Pages** (Deployment automatisch bei jedem Push zu GitHub).

- **Live-Adresse:** die kostenlose Cloudflare-Pages-Adresse **`cognizance-website.pages.dev`** (+ 2 angehängte Domains).
- **Eigene Domain:** ⚠️ **im Umbruch** — siehe Abschnitt 7. Aktuell **keine** feste eigene Domain zugewiesen.
- **GitHub:** github.com/gordongeggo/cognisance-website · **Ordner:** `cognisance-website` (die „s/z"-Schreibweise ist rein kosmetisch).
- **Inspiration (Ursprung):** die Orano-Innovations-Seite (`orano.group/experience/innovation/en`) — ein Echtzeit-Code-Erlebnis, Vorbild fürs „lebendige" Gefühl.

## 2. Über den Entwickler & Arbeitsweise (WICHTIG)

**Ronny ist absoluter Programmier-Anfänger.** Für jede Zusammenarbeit gilt:
- Jeden Schritt **VORHER in einfachem Deutsch erklären**, keine Fachbegriffe ohne Erklärung.
- **Qualität vor Tempo — „Hier gibt es kein schnell, nur Qualität."** Kein Zeitdruck; eine Sequenz darf einen Tag oder eine Woche dauern. **Nie heimlich abkürzen** — wenn etwas länger dauert, **vorher** ehrlich sagen.
- **Immer auf ein ausdrückliches „Go" warten:** erst erklären → Rückfragen → Ronnys Go → **DANN** bauen. **Keine eigenmächtigen kreativen oder Scope-Entscheidungen.**
- **Kleine Schritte**, nach jedem ein sichtbares Ergebnis; jede Änderung mit **Git-Commit** sichern.
- **Präzision in der Sprache ist Pflicht.** Nie behaupten, etwas erreicht/gesehen zu haben, das man nicht wirklich erreichen kann. Bekanntes klar von Vermutetem trennen.
- **Git-Identität:** Ronny Hammer / ronny.hammer1@icloud.com

**Was der claude.ai-Chat (HOME-Watson) sehen kann (präzise):** die **Text-Dateien im Projekt** (`.md`, `.docx`, `.pdf`) und **direkt in den Chat hochgeladene Bilder**. **NICHT** sichtbar: der laufende Code, die **Videos** (Bewegung ist im Chat unsichtbar) und Dateien im **Schreibtisch-Ordner**. Damit der HOME-Watson auf Stand ist, wird **genau dieses Dokument** aktuell gehalten und ins Projekt geladen.

**Veröffentlichen:** Änderung an `index.html` → committen → zu GitHub pushen → Cloudflare Pages baut automatisch neu (1–2 Min.) → im Browser mit **Cmd+Shift+R** hart neu laden.

**Werkzeug-Aufteilung:** Technische Arbeit (Code, Git, Cloudflare, Video-Umwandlung) passiert in **Claude Code**. Der claude.ai-Chat ist für **Planung, Architektur, Dokumentation** und fürs gemeinsame **Firefly-/Video-Prompten**.

## 3. Technik

- **Startseite:** zwei eingebettete Videos (`<video>`) + eine **Code-Overlay-Schicht** + eine **WebGL-Gravitationslinse** auf Video 1. Bewusst **kein** Echtzeit-WebGL-Flug mehr.
- **Menü, Kapitel, Navigation, Overlay:** **Vanilla JS + HTML5/CSS**, keine Frameworks.
- Alles steckt in **einer Datei**: `index.html` (HTML + CSS + JS zusammen).
- **Farbwelt:** samtiges Schwarz-Blau (#030308 / #080815), Gold **#d4af37**, Violett **#b19ffb**, Sternenweiß.
- **Desktop-fokussiert** (die Linse nutzt WebGL). Es gibt einen **Rückfall**: kann der Browser das lokale Video nicht in die Linse einlesen (z. B. Doppelklick/`file://`) oder fehlt WebGL, zeigt der Code **Video 1 einfach normal** (ohne Linsen-Biegung). Live über HTTPS läuft die Linse voll.

## 4. Verbindliche Design-Identität (gilt für ALLE Seiten)

- **Präzise und mathematisch statt verspielt.** Exakte Geometrie, klare Konstruktion. Möglichst **kein zufälliger „Staub"**.
- **Typografie:** scharf, dünn (font-weight 100–300), weit gesperrt, Großbuchstaben für Titel.
- **Leitmotiv „Holodeck-Gitter":** ein leeres, perspektivisches Liniengitter als „Struktur hinter der Realität".
- **Durchgehende Farb-Harmonie:** die Farbe fließt über die **ganze** Seite — vom blauen Quanten-Netz (Video 1) über den Flug (Video 2) bis zur Portal-Seite. Fließende Übergänge, keine harten Farbbrüche; das Ganze mündet ins dunkle `#080815`.

## 4a. Das Portal-Menü — FERTIG und (bis auf Überschriften) TABU

Die Seite mit den **vier Toren** ist **fertig**. Einzige mögliche spätere Ausnahme: die **Überschriften** der Portale.

**Menü „Vier Tore der Erkenntnis":**
- **I. Die Illusion der Zeit** → Kapitel I fertig (Einstein-Zitat).
- **II. Außerirdische Intelligenz** → Platzhalter-Seite (Inhalt folgt).
- **III. Realität als Projektion** → Platzhalter-Seite (Drehbuch siehe Abschnitt 6).
- **IV. Wachstum durch KI** → Platzhalter-Seite (Inhalt folgt).

**Navigation (fertig & live):** „← Zu den Toren" auf jeder Kapitel-/Platzhalterseite; „Andere Tore: I II III IV"-Sprunglinks (auch in Kapitel I); „↻ Von vorn" (lädt die Seite neu, das ganze Intro startet von vorn).

**Ceremonieller Aufbau (umgebaut 15. Juli 2026 — „UFO-Einflug", ~17 Sek.):**
Schriftzug und Einflug laufen **parallel** — ruhiges Licht oben gegen scharfe Bewegung in der Mitte.
1. **Sek. 1,0–6,0: „Cognizance World"** erglüht **als GANZES**, gemächlich: eine einzige Bewegung
   aus der Unschärfe herauf, kurzes violettes Aufglimmen, dann setzt er sich. *(Kein Buchstabe-für-
   Buchstabe mehr — das flackerte, weil ständig 4–5 Buchstaben in verschiedenen Stadien überlappten.)*
   Der Schriftzug ist **responsiv**: auf dem Desktop unverändert, auf schmalen Handys schrumpft er
   automatisch, damit er nie über den Rand steht.
2. **Sek. 2,6–8,2 (parallel dazu): der UFO-Einflug.** Die 4 Kreise schießen nacheinander ins Bild
   (Flug je 0,42 s, **1,3 s Pause dazwischen**), jeder mit **gerichtetem Bewegungsschlier**,
   **abruptem Stopp** und **Einrast-Blitz**. Reihenfolge/Richtung: **I** von rechts (→ oben links),
   **II** von unten (→ oben rechts), **IV** von links (→ unten rechts), **III** von unten (→ unten links).
3. **Sek. 7,0:** der Untertitel **„Vier Tore der Erkenntnis"**.
4. **Ab Sek. 9,0 — erst wenn alle 4 Scheiben stehen** — erwachen die **Ziffern** langsam, **in
   zufälliger Reihenfolge, nie I→II→III→IV**; jede Bezeichnung folgt ihrer eigenen Ziffer; die Tore
   **schweben** sanft (versetzt, nicht im Gleichschritt). Ende bei ~17,3 Sek.
- Feines **Hintergrund-Gitter** (Holo-Gitter, ~5 % Deckkraft).
- **Klick irgendwo während der Zeremonie** = überspringen, sofort das fertige Menü.
- **Wiedererkennung:** erster Besuch → volle Zeremonie; jeder weitere Besuch → direkt das fertige
  Portal (`localStorage`). **„↻ Von vorn" zeigt immer wieder die volle Zeremonie.**
- **Alle Timings stehen gesammelt im `CFG`-Block** ganz oben im `<script>` und sind leicht justierbar.
  Wichtigste Schrauben: `WORD_GLOW` (wie gemächlich der Schriftzug erglüht), `ORB_FLY_GAP` (Ruhe
  zwischen den Einflügen) und **`ORB_START`** — *eine* Zahl entscheidet über parallel (2.6) oder
  streng nacheinander (8.0).

## 5. Was live läuft (Ist-Zustand in `index.html`)

**Die interaktive Video-Startseite (Abschnitt 5a) ist LIVE.** Ablauf: Video 1 (Netz) + Gravitationslinse → „ERKENNE" halten → Lichtblitz → Video 2 (Flug) → ab Sek. 9 abdunkeln → Portal-Menü (ceremoniell) → klickbar.

*(Das alte WebGL-Schwarze-Loch-Intro ist damit ersetzt und nicht mehr live. Siehe Abschnitt 5b.)*

## 5a. Die Video-Startseite — GEBAUT & LIVE (13. Juli 2026)

**Grundidee:** Die Seite ist vom ersten Moment an **lebendig** und **interaktiv**. Der Besucher **löst den Flug selbst aus** — der Beobachter-Effekt, um den sich das Projekt dreht.

### Der Ablauf (die Kette) — alles gebaut
1. **Video 1 — Ambient-Schleife** (`video1.mp4`) läuft sofort, endlos, **stumm**, Autoplay-Loop. Das blaue Quanten-Netz. **Web-Version 1080p / 4,9 MB**, aus dem gekauften 4K-Original (`AdobeStock_430161342.mov`, 62,7 MB) mit macOS-`avconvert` gerechnet. Die 4K-Datei bleibt **lokal** (via `.gitignore` ausgeschlossen, > 25 MB).
2. **Overlay (Code) über Video 1:**
   - **Gravitationslinse** (WebGL): eine weiche Raumzeit-Delle biegt das Netz, **folgt dem Mauszeiger** und **vertieft sich beim Halten** von „ERKENNE". Dezent/real (keine Singularität, kein bunter Ring). Mit Rückfall (Abschnitt 3).
   - **„ERKENNE"-Ritual** in der Mitte: **Klick-und-Halten** lädt einen goldenen Ring (~1,4 Sek.), bei **100 %** → Video 2. (Bewusst „Ritual", nicht bloßer Klick.)
3. **Video 2 — der Flug** (`netz_kling_v1.mp4`, Kling 3.0, 13,9 MB) spielt **einmal**: atmendes Quanten-Netz, aus dem eine geometrische Figur aufsteigt (**kein** Wurmloch). **Ton erlaubt** (kommt später).
4. **Portal-Seite** erscheint aus dem `#080815` und baut sich ceremoniell auf (Abschnitt 4a).

### Die zwei „Nähte" (unsichtbare Übergänge) — gebaut
- **Naht 1 (Video 1 → Video 2):** im Umschaltmoment legt der Code einen **hellen Lichtblitz** aus der Mitte darüber, der den Schnitt überstrahlt. *(Zusätzlich sicherbar über Frame-Matching: erstes Bild von Video 2 = Ruhebild der Schleife, `Video_1.png`.)*
- **Naht 2 (Video 2 → Portal):** Das Video klingt **NICHT von selbst schwarz aus.** **Der Code dunkelt ab Sekunde 9** einen Schleier von durchsichtig auf voll deckend, **Zielfarbe = `#080815`** (nicht reines Schwarz), **spätestens bei Video-Ende (Sek. 10) voll**. **Erst dann** öffnet die Portal-Seite. *(Timing im Code justierbar.)*

### Schriftzug „Cognizance World"
- **Gebaut** als **Code-Overlay auf der Portal-Seite** (nicht ins Video eingebrannt), in Ronnys Stil (dünn, gesperrt, Großbuchstaben). Erscheint **Buchstabe für Buchstabe aus der Mitte heraus** (Alien-Titel-Stil). Text jederzeit änderbar.

### Reine Referenz/Produktion (wie Video 2 entstand — Firefly/Kling)
- **Video 2 gefunden mit Kling 3.0** (nach vielen Runden). Kein Modell (Veo 3.1, Kling, Ray/Ray HDR) konnte eine **exakte Wurmloch-Röhre** zuverlässig — die Schwäche der KI-Video-Modelle ist *exakte Geometrie*. Der Netz-Flug passt sogar besser zur Design-Identität.
- **Firefly-Erkenntnisse (für künftige Videos):** Adobe-eigenes Modell schwächer → Partner-Modelle (Kling 3.0 / Veo 3.1 / Runway Gen 4.5; **Sora 2 meiden**). **Startbild `Video_1.png`, KEIN Endbild** (Endbild sperrt Kamerabewegung). **16:9, 1080p.** Ton später via „Generate sound effects".
- **Referenz-Dateien (im claude.ai-Projekt):** `Video_1.png` (Ruhebild/Startbild), `schwarzes_Ende.png`, `Page_Seite_2_.png` (Portal-Farbvorlage).

### Echte Farbwerte der Portal-Seite (für Prompts & Code)
- **Hintergrund:** radial `#080815` (Mitte) → `#010103` (Rand); Grundton `#030308`.
- **Holo-Gitter-Linien:** `rgb(130,175,245)` bei ~5 % Deckkraft. **Gold:** `#d4af37` · **Violett:** `#b19ffb`.

## 5b. Frühere Code-Wege (WebGL-Schwarzes-Loch & Platinen-Hybrid) — HISTORIE / pausiert

> **Status:** durch die Video-Startseite abgelöst. Dateien bleiben erhalten (nichts gelöscht).

- Das **WebGL-Schwarze-Loch-Intro** war eine Zeit lang live, ist jetzt **ersetzt**.
- Der **Platinen-/Chip-Hybrid** („Flug rückwärts zum Ursprung": Projektion → Tunnel → Hardware/Platine → Chip = Menü; Bedeutungskette **Hardware → Programm → Projektion**; schwarzes Loch rein / weißes Loch raus als Unsterblichkeits-Kreislauf) liegt als **Werkstatt-Preview** in **`neues-intro.html`** (Teil 1 „Blick zurück auf schrumpfenden Eingang" gebaut, Teile 2–4 nicht). Als Ideen-Reserve behalten.
- **`video-preview.html`** war die Werkstatt-Preview der Video-Startseite (jetzt in `index.html` übernommen; die Datei kann später aufgeräumt werden).

## 6. Drehbuch: Portal III „Realität als Projektion" (Holodeck) — noch zu bauen

Ziel: Der Besucher *erlebt* die Simulationshypothese. Technik: Vanilla JS + Canvas, mobilkompatibel.

- **Phase A – Leerer Raum:** perspektivisches **Gold-Liniengitter** (Fluchtpunkt Bildmitte), minimale Maus-Parallaxe. Text: „WAS DU REALITÄT NENNST, IST EINE PROJEKTION." Darunter klein: „Erzeuge sie."
- **Phase B – Der Befehl:** feiner goldener Kreis „PROJIZIERE" (Click-and-Hold wie „ERKENNE").
- **Phase C – Rendern:** bei 100 % baut sich „Realität" ÜBER dem Gitter auf (Lichtflecken → Sterne → Nebel → Texte). Gitter verblasst, verschwindet aber **nie ganz** (~3–5 %).
- **Phase D – Durchschauen (Kern):** bei Mausbewegung schimmert das Gitter um den Cursor wieder durch. Metapher: der aufmerksame Blick entlarvt die Simulation.
- **Phase E – Inhalt:** 2–3 philosophische Fragmente, z. B. „Vielleicht ist Mathematik keine Beschreibung der Welt. Vielleicht ist sie ihr Quellcode."

## 7. Infrastruktur (⚠️ IM UMBRUCH)

- Die drei Domains `theholographicme.com`/`.de`/`.global` wurden **aus Cloudflare entfernt**. Ronny hat **5 neue Domains**; welche fürs Projekt, ist **noch offen**.
- **Cloudflare-Pages-Projekt läuft weiter**, erreichbar über `cognizance-website.pages.dev` (+ 2 Domains). Zum Testen reicht das.
- **DMARC / E-Mail-Schutz** und **Cloudflare Access (Login „Nur ich")** hingen an den entfernten Domains — **vermutlich mit-weg, zu prüfen** nach Domain-Wahl.
- **Cloudflare-MCP:** `.mcp.json` deckt Workers/Storage ab, **nicht** DNS/Zone oder Pages-Deploy-Status.

## 8. Offene Aufgaben / nächste Ziele

- **Feinschliff der Timings** der Startseite (Ladezeit „ERKENNE", Naht-Tempo, Portal-Choreografie) — nach Ronnys Gefühl, alles leicht justierbar.
- **Inhalte für Portale II & IV** (aktuell Platzhalter).
- **Portal III (Holodeck)** bauen — Drehbuch Abschnitt 6.
- **Sound für Video 2** (Firefly „Generate sound effects").
- **Video-Dateigröße** ggf. weiter optimieren (aktuell Video 1 = 4,9 MB, Video 2 = 13,9 MB — beide ok für Cloudflares 25-MB-Grenze).
- **Domain-Entscheidung:** eine der 5 neuen Domains auswählen und dem Pages-Projekt zuweisen; danach **DMARC/Access prüfen** (Abschnitt 7).
- Optional: `video-preview.html` / `neues-intro.html` aufräumen; JS aus `index.html` in `script.js` auslagern.

## 9. Changelog

- **15. Juli 2026 (später) — ZEREMONIE NACHGESCHLIFFEN (Ronnys Rückmeldung).** (8) Der Schriftzug
  erglüht jetzt **als Ganzes** statt Buchstabe für Buchstabe (Animation von `.ch` auf `#wordmark`
  verlegt, `chIgnite` → `wmIgnite`, 5,0 s). Grund fürs Flackern war der Rhythmus: alle 0,5 s zündete
  ein Buchstabe über 2,2 s → es überlappten ständig 4–5 in verschiedenen Stadien. Jetzt: **eine**
  Bewegung (geprüft: 1 Animation statt 15). Die Buchstaben-Kästchen bleiben und halten das exakte
  Schriftbild. (9) **`ORB_FLY_GAP` 0,22 → 1,3 s** (Flugdauer bleibt 0,42 = „blitzschnell mit abruptem
  Stopp"); `ORB_DELAY` ersetzt durch **`ORB_START`** = fester Zeitpunkt ab Zeremonie-Beginn, damit der
  Einflug **parallel** zum Schriftzug laufen kann (2.6 = parallel, 8.0 = nacheinander — eine Zahl).
  `N_START` nimmt `Math.max(circlesEnd, subEnd)`, damit die Ziffern immer auf beides warten.
  **Zeremonie: 30 → 24 → ~17,3 Sek.**
- **15. Juli 2026 — PORTAL-ZEREMONIE UMGEBAUT („UFO-Einflug").** In 7 kleinen Schritten, je ein Commit:
  (1) Schriftzug **responsiv** (Desktop beweisbar unverändert; 375 px → Faktor 0,91, 320 px → 0,87;
  `ResizeObserver` statt `resize`-Event). (2) Buchstaben **fest an Ort und Stelle**, Aufleuchten in
  **zufälliger Reihenfolge** (`shuffled()`, Fisher-Yates; Zoom-Bewegung entfernt). (3) **UFO-Einflug**
  I→II→IV→III mit Start außerhalb des Bildes (CSS-Variablen `--fx/--fy`), Landung exakt auf der alten
  Position. (4) **Gerichteter Bewegungsschlier** (SVG-Filter `#trail-x`/`#trail-y`, `stdDeviation "18 0"`
  bzw. `"0 18"` — ein normaler `blur()` sähe nach Nebel aus) + **Einrast-Blitz**, der exakt auf die
  Originalwerte zurückfällt. (5) **Ziffern gewürfelt**, `shuffledStrict()` sperrt I→II→III→IV (bei nur
  4 Ziffern käme sie sonst in ~jedem 24. Besuch; über 3000 Testläufe: 0×, genau die 23 übrigen
  Reihenfolgen, gleichverteilt). (6) **Klick überspringt** (alle Zeitschalter über `at()` sammelbar,
  `#portal.instant` nimmt nur den Aufbau-Bewegungen die Dauer — das Schweben läuft weiter; Abbruch-Klick
  in der capture-Phase, damit er kein Tor öffnet). (7) **Wiedererkennung** über `localStorage`;
  „Von vorn" hinterlegt eine einmalige `sessionStorage`-Notiz und zeigt die volle Zeremonie.
  **Video-Kette nachweislich unangetastet** (kein Diff an Video 1/2, Linse, Ritual, Blitz, Naht 2).
  Dauer der Zeremonie: **~30 → ~24 Sek.** (der Einflug allein: 13,6 → 2,3 Sek.).
- **13. Juli 2026 (Nacht) — VIDEO-STARTSEITE LIVE.** Komplette neue `index.html` gebaut, integriert und deployed: Video 1 (`video1.mp4`, aus 4K-`.mov` via `avconvert` auf 1080p/4,9 MB) + **Gravitationslinse** (WebGL, weiche Delle, folgt Maus, vertieft beim Halten; **mit Rückfall** für `file://`/kein-WebGL) + **„ERKENNE"-Ritual** → **Lichtblitz (Naht 1)** → **Video 2** (`netz_kling_v1.mp4`, 13,9 MB) → **Naht 2** (Code dunkelt ab Sek. 9 auf `#080815`) → **Portal-Menü** ceremoniell (Schriftzug „Cognizance World" Buchstabe-für-Buchstabe aus der Mitte, dann Kreise einzeln, dann Ziffern) → **voll klickbar** (Kapitel I, Platzhalter II–IV, Navigation, „Von vorn"). Ersetzt das WebGL-Schwarze-Loch-Intro. Beide Videos im Repo, 4K-Original via `.gitignore` ausgeschlossen. Getestet, keine Fehler.
- **13. Juli 2026:** Naht-2-Widerspruch in der Doku bereinigt (Video klingt **nicht** von selbst schwarz aus; Code dunkelt ab Sek. 9 auf `#080815`).
- **13. Juli 2026:** **Video 2 gefunden** (Kling 3.0: atmendes Quanten-Netz → aufsteigende Figur; Wurmloch verworfen, weil KI-Video keine exakte Geometrie schafft). Startseite als **Zwei-Video-Architektur** festgelegt (Video 1 Ambient-Loop + Overlay + Video 2 Flug + Nähte).
- **11. Juli 2026:** Grundsatz-Entscheidung: Startseite als eingebettetes Video statt WebGL. Recherche: „Video → lesbarer Code" geht nicht; Lottie nur für Vektor.
- **9. Juli 2026:** WebGL-Schwarze-Loch-Intro fertig & integriert (später abgelöst); Navigations-Buttons + Platzhalterseiten II–IV; Platinen-Hybrid-Teil-1 in `neues-intro.html`; Arbeitsregel „Qualität vor Tempo, auf Go warten" festgehalten; alle `theholographicme`-Domains aus Cloudflare entfernt (Infrastruktur „im Umbruch").
- *(früher)* cognizance.world → theholographicme.com; Auge-des-Beobachters-Intro; Wurmloch (4D-Tesserakt); DMARC repariert; Website zeitweise privat via Access.
