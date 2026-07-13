# TheHolographicMe — Projekt-Übergabe & Zusammenfassung

> **Eine Datei für alles.** Dieses Dokument ist die *einzige* aktuelle Projekt-Übersicht.
> Es ersetzt die vorherige `PROJEKT-ZUSAMMENFASSUNG.md`. Du kannst es in einen anderen
> Claude-Chat oder als Wissensquelle in dein claude.ai-Projekt hochladen.
> **Stand: 13. Juli 2026 (aktualisiert – Video 2 gefunden; Naht-2-Widerspruch korrigiert).**

---

## 0. Das Wichtigste zuerst (aktueller Stand & nächster Schritt)

Die Startseite wird **interaktiv** und besteht aus **zwei Videos + einer Code-Schicht (Overlay)**.
Das Portal-Menü mit den vier Toren **bleibt unangetastet** (Abschnitt 4a).

**Fertig und bereit zum Hochladen ins GitHub: Video 1** — die **Ambient-Schleife** (gekauft, perfekte
nahtlose Endlosschleife, Ende = Anfang, kein Ruckeln). Sie läuft sofort beim Laden und ist der ruhige,
wartende Zustand.

**Nächster Job für den Watson im Code:** das **Overlay** über Video 1 codieren — der **leuchtende
Klick-und-Halte-Auslöser in der Bildmitte** mit **Gravitationslinsen-Effekt** auf das Netz darunter
(Details in Abschnitt 5a). Das kann **sofort** gebaut werden, unabhängig von Video 2, weil das Overlay
auf Video 1 liegt.

**GEFUNDEN & abgesegnet: Video 2** — der Startseiten-Flug. **NICHT** das Wurmloch (das hat kein
Modell zuverlässig hinbekommen), sondern ein **atmendes Quanten-Netz, aus dem eine geometrische
Figur aufsteigt** (Details + Historie in Abschnitt 5a). Erzeugt in **Kling 3.0**. Muss als Datei
gesichert und später in `index.html` eingebunden werden.

---

## 1. Was ist das Projekt?

Ein interaktives digitales **Kunstwerk über Wahrnehmung, Quantenphysik und Bewusstsein**.
Eine einzelne, statische Website, live über **Cloudflare Pages** (Deployment automatisch
bei jedem Push zu GitHub).

- **Live-Adresse aktuell:** die kostenlose Cloudflare-Pages-Adresse `…pages.dev` (das Pages-Projekt läuft weiter, unabhängig von Domains).
- **Eigene Domain:** ⚠️ **im Umbruch** — siehe Abschnitt 7. Es ist aktuell **keine** eigene Domain zugewiesen.
- **Früher:** cognizance.world (abgelöst) und danach theholographicme.com (siehe Changelog / Abschnitt 7).
- **GitHub:** github.com/gordongeggo/cognisance-website · **Ordner:** `cognisance-website` (die „s/z"-Schreibweise ist rein kosmetisch)
- **Inspiration (Ursprung):** die Orano-Innovations-Seite (`orano.group/experience/innovation/en`). Wichtig zu wissen: Das ist ein **Echtzeit-Code-Erlebnis (WebGL)**, kein Video — daher das lebendige Reagieren auf die Maus. Das ist das Vorbild für das „lebendige" Gefühl, nicht als Video kopierbar.

## 2. Über den Entwickler & Arbeitsweise (WICHTIG)

**Ronny ist absoluter Programmier-Anfänger.** Für jede Zusammenarbeit gilt:
- Jeden Schritt **VORHER in einfachem Deutsch erklären**, keine Fachbegriffe ohne Erklärung.
- **Qualität vor Tempo — „Hier gibt es kein schnell, nur Qualität."** Kein Zeitdruck; eine einzelne Sequenz darf ruhig einen Tag oder eine Woche dauern. **Nie heimlich abkürzen** – wenn etwas länger dauert, **vorher** ehrlich sagen.
- **Immer auf ein ausdrückliches „Go" warten:** erst erklären → Rückfragen → Ronnys Go → **DANN** bauen. **Keine eigenmächtigen kreativen oder Scope-Entscheidungen.**
- **Kleine Schritte**, nach jedem ein sichtbares Ergebnis; jede Änderung mit **Git-Commit** sichern.
- **Präzision in der Sprache ist Pflicht.** Nie behaupten, eine Datei/einen Ort erreicht zu haben, den man nicht wirklich erreichen kann. Was aus Uploads bekannt ist, klar trennen von dem, was vermutet/gefolgert ist.
- **Git-Identität:** Ronny Hammer / ronny.hammer1@icloud.com

**Was der claude.ai-Chat sehen kann (präzise):** Die **Text-Dateien im Projekt** (`.md`, `.docx`,
`.pdf`) und **direkt in den Chat hochgeladene Bilder** liegen im Kontext und können gelesen/gesehen
werden. **NICHT** sichtbar sind: der tatsächliche Code in `index.html` / `neues-intro.html`, die
**fertigen Videos** (Bewegung ist für den Chat unsichtbar) und Dateien im **Schreibtisch-Ordner**.
Wenn Claude im Chat ein Bild sehen soll, muss es **direkt in den Chat hochgeladen** werden.

**Veröffentlichen:** Änderung an `index.html` → committen → zu GitHub pushen →
Cloudflare Pages baut automatisch neu (1–2 Min.) → im Browser mit **Cmd+Shift+R** hart neu laden.

**Werkzeug-Aufteilung:** Die technische Arbeit (Code, Git, Cloudflare) passiert in **Claude Code**.
Der claude.ai-Chat ist für **Planung, Architektur, Dokumentation** (dieses Dokument) sowie fürs
Ansehen hochgeladener Bilder und fürs gemeinsame **Firefly-Prompten**.

## 3. Technik

- **Vanilla JavaScript + HTML5-Canvas**, keine Frameworks, `requestAnimationFrame` — für Menü + Kapitel + das Overlay (mobilkompatibel).
- **Startseite = zwei eingebettete Videos (`<video>`) + eine Code-Overlay-Schicht darüber.** Details in Abschnitt 5a. Bewusst **kein** Echtzeit-WebGL-Flug mehr.
- Aktuell steckt **alles in einer Datei**: `index.html` (HTML + CSS + JavaScript zusammen).
- **Farbwelt:** samtiges Schwarz-Blau (#030308 / #080815), Gold **#d4af37**, Violett **#b19ffb**, Sternenweiß.

## 4. Verbindliche Design-Identität (gilt für ALLE Seiten)

Das Menü nach dem Eingang und die Kapitel-I-Seite definieren die visuelle Identität:
- **Präzise und mathematisch statt verspielt.** Exakte Geometrie, klare Konstruktion. Möglichst **kein zufälliger „Staub"**, keine wolkige Verspieltheit.
- **Typografie:** scharf, dünn (font-weight 100–300), weit gesperrt, Großbuchstaben für Titel.
- **Leitmotiv „Holodeck-Gitter"** (Star-Trek-inspiriert): ein leeres, perspektivisches Liniengitter als „Struktur hinter der Realität". Die sichtbare Welt ist nur eine Projektion darüber.
- **Durchgehende Farb-Harmonie (Entscheidung 13. Juli):** Die Farbe soll über die **ganze** Seite fließen — vom blauen Quanten-Netz (Video 1) über den Flug (Video 2) bis zur Portal-Seite. Ein **fließender Übergang**, keine harten Farbbrüche. Das Wurmloch wird farblich in *Ronnys* Palette geholt (Schwarz-Blau, Gold, Violett) statt warm-orange, und trägt **am Ende des Fluges die Farben der Portal-Seite**, bevor es ins Schwarz geht.

## 4a. Das Portal-Menü — FERTIG und TABU

Die Seite mit den **vier Toren** ist **fertig, perfekt und wird nicht mehr verändert** —
einzige mögliche spätere Ausnahme: die **Überschriften** der Portale.

**Menü „Vier Tore der Erkenntnis":**
- **I. Die Illusion der Zeit** → Kapitel I fertig (Einstein-Zitat), öffnet sich langsam (4,5 Sek.)
- **II. Außerirdische Intelligenz** → Platzhalter-Seite (Inhalt folgt)
- **III. Realität als Projektion** → Platzhalter-Seite (Drehbuch siehe Abschnitt 6)
- **IV. Wachstum durch KI** → Platzhalter-Seite (Inhalt folgt)

**Navigation (fertig):** „← Zu den Toren" auf jeder Kapitel-/Platzhalterseite, „Andere Tore: I II III IV"-Sprunglinks, „↻ Von vorn" (Intro neu).

## 5. Was heute wirklich live läuft (Ist-Zustand in `index.html`)

> Dieser Ist-Zustand **wird durch die neue Startseite (Abschnitt 5a) ersetzt**, bleibt aber als
> stabile Live-Version bestehen, **bis** die neue Video-Startseite fertig und abgesegnet ist.
> **Nichts wird gelöscht, nichts überschrieben, bevor der Ersatz steht.**

Aktuell läuft in `index.html` das alte **WebGL-Schwarze-Loch-Intro**: fernes gelinstes Schwarzes Loch
→ Maus-Sog → Auto-Flug ins Loch → Gitter-Tunnel → Projektionsfläche dreht sich gerade → Portal-Menü.
Der **Wurmloch-Tunnel** und das **Projektionsflächen-Ende** waren bereits vorher von Ronny abgelehnt.

## 5a. Die neue Startseite — interaktiv, zwei Videos + Overlay (Stand 13. Juli 2026)

**Grundidee:** Die Seite ist vom ersten Moment an **lebendig** und **interaktiv** (Gegenteil eines
still ablaufenden Videos). Der Besucher **löst den Flug selbst aus** — das ist der Beobachter-Effekt,
um den sich das ganze Projekt dreht: Realität geschieht erst durch die Handlung des Betrachters.

### Der Ablauf (die Kette)
1. **Video 1 — Ambient-Schleife** läuft sofort beim Laden, endlos, ruhig, **stummgeschaltet**
   (Browser erlauben Auto-Start nur bei stummem Video). Zeigt den wartenden Zustand: das blaue
   Quanten-Netz. **Status: FERTIG & gekauft**, perfekte nahtlose Schleife (Ende = Anfang).
2. **Overlay (Code, über Video 1)** — ein **leuchtender Auslöser in der Bildmitte**:
   - reagiert auf die Maus (glüht auf beim Annähern),
   - **Klick-und-Halten** lädt ihn auf (kreisrunder Ladebalken, das „Ritual" wie in der allerersten
     HTML-Version — bewusst gewählt, **nicht** „jede Mausbewegung", **nicht** einfacher Klick),
   - verbiegt das Netz darunter wie eine **echte Gravitationslinse** (Linien krümmen sich um ihn),
   - bei **100 % Ladung** → löst **Video 2** aus.
   - **Wichtig:** Der Auslöser ist **Code**, nicht ins Video gerechnet (ein Video kann die Maus nicht
     sehen; Video 1 ist zudem gekauft und tabu). → **Das ist der nächste Bau-Job im Code.**
3. **Video 2 — der Flug** spielt **einmal** ab (der Kling-3.0-Flug: atmendes Quanten-Netz → aufsteigende
   Figur, **kein** Wurmloch). Es **klingt NICHT von selbst schwarz aus** — **der Code** dunkelt es **ab
   Sekunde 9** in die Portalfarbe `#080815` ab (Details in „Naht 2 — final festgelegt"). **Ton erlaubt**
   (der Klick des Besuchers ist die „Autoplay-Erlaubnis" des Browsers) — Sound kommt aber erst später (Abschnitt 5a, „Ton").
4. **Portal-Seite erscheint aus dem Schwarz** — die echte, klickbare Seite mit den vier Toren.

### Die zwei „Nähte" (unsichtbare Übergänge)
- **Naht 1 (Video 1 → Video 2):** Kombi aus **B + C**.
  **(B)** Video 2 **beginnt genau im Ruhezustand von Video 1** — das erreicht Ronny, indem er in
  Firefly das **erste Bild von Video 2 = das Ruhebild der Schleife** setzt (`Video_1.png`).
  **(C)** Im Umschaltmoment legt der Code einen **hellen Lichtblitz / eine Druckwelle** aus der Mitte
  darüber, der den Schnitt **überstrahlt** (alter Filmtrick: wo es blitzt, sieht man den Schnitt nicht).
- **Naht 2 (Video 2 → Portal-Seite):** Das Video **klingt NICHT von selbst schwarz aus.** Stattdessen legt
  **der Code ab Sekunde 9** einen **Schleier** über das Bild (durchsichtig → voll deckend), **Zielfarbe =
  Portal-Hintergrund `#080815`** (nicht reines Schwarz), **spätestens bei Video-Ende (Sek. 10) voll deckend**.
  **Erst dann** öffnet sich die Portal-Seite aus diesem `#080815`. So bestimmt Ronny den Schluss, nicht
  Firefly. (Ausführlich unten: „Naht 2 — final festgelegt (13. Juli)".)

### Schriftzug „Cognizance World"
- **NICHT ins Video einbrennen.** Gründe: KI-Video schreibt Text notorisch fehlerhaft; eingebrannter
  Text ist unveränderlich und trifft den Hausstil nicht. **Stattdessen als Code-Overlay** in exakt
  Ronnys Stil (dünn, weit gesperrt, Großbuchstaben, Gold/Violett), jederzeit änderbar.
- **Offen:** ob und wo der Schriftzug erscheint (evtl. erst auf **Seite 2 / Portal-Seite**). Ronny
  entscheidet später. Kein Zeitdruck.

### Firefly-Einstellungen für Video 2 (der Flug)
- **Modell:** **Veo 3.1** (erster Versuch). Das **Adobe-eigene** Firefly-Modell ist schwächer — daher
  eins der **Partner-Modelle**. Reihenfolge, falls Veo 3.1 enttäuscht: **Kling 3.0 Omni** (treueste
  Übernahme des Vorlage-Looks) als 2. Wahl; **Runway Gen 4.5** (Kamera-Kontrolle, aber die besten
  Regler leben in Runways eigener App, evtl. nicht voll in Firefly). **Sora 2 meiden** (wird
  eingestellt). Praxis-Tipp: denselben Prompt bei Unzufriedenheit durch ein zweites Modell jagen und
  vergleichen (Credits sind vorhanden).
- **Referenz-Bilder:** **erstes Bild (First) = `Video_1.png`** (sichert Naht 1). **Kein Endbild (Last)**
  — ein festes Endbild würde in Firefly **Kamera-Bewegungen deaktivieren**, die wir für den Flug (und
  später die Abzweigungen) brauchen. Das Schwarz am Ende kommt über **Prompt + Code-Schleier**, nicht
  über ein Endbild.
- **Format/Auflösung/Dauer:** **16:9**, **1080p** (reicht auch für größere Bildschirme, bleibt leichter
  als 4K), **8 Sekunden** (bewusst statt 6; kein Schnitt in Premiere gewünscht).
- **Ton:** **später** über Fireflys „Generate sound effects". Nur Video 2 darf Ton haben (Video 1 läuft
  stumm wegen Autoplay).

### Video 2 — GEFUNDEN (Stand 13. Juli, nach vielen Runden)

**Ergebnis:** Der Startseiten-Flug ist **kein Wurmloch** mehr. Kein Modell (Veo 3.1, Kling, Ray/Ray HDR)
konnte die gewünschte **schlauchförmige, abgegrenzte, transparente Wurmloch-Röhre mit Krümmungen**
zuverlässig erzeugen — mal wurden es Striche, mal Ringe, mal ein bildschirmfüllender Warp. **Ehrliche
Erkenntnis:** eine *exakte geometrische Form* ist die Schwäche dieser KI-Video-Modelle (Stimmung/Licht/
Weltraum: super; „genau diese Form": Glücksspiel). Abzweigungen ebenfalls nicht machbar in einem Clip.

**Der Flug, der funktioniert (Kling 3.0):** ein **atmendes Quanten-Netz** (auf/ab, wie Atmen), aus dem
sich eine **geradlinige, nach oben spitz zulaufende geometrische Figur** erhebt (wie eine Fontäne), aus
der **Sterne entspringen und verblassen**. Präzise, geometrisch, ruhig — passt **perfekt zur Design-
Identität** (Holodeck-Gitter, aus dem Struktur entsteht). Besser als das Wurmloch je gepasst hätte.

- **Länge: 10 Sekunden.** **Ab Sekunde 9** werden die Sterne weniger, schwächer, sinken nach unten —
  das Video bereitet den ruhigen Ausklang selbst vor.
- **Modell: Kling 3.0** (nicht Omni nötig). **Als beste Datei sichern** (`netz_kling_final.mp4`) — Kling
  liefert das **nie wieder exakt so**.
- **Ende bewusst NICHT in Firefly erzwungen** — das Abdunkeln in die Portalfarbe macht der Code (s. u.,
  Naht 2). Das Video darf mit ein paar Sternen ausklingen; das reicht.

### Naht 2 (Video 2 → Portal-Seite) — final festgelegt (13. Juli)
Ablauf **nacheinander** (bewusst, damit nichts abrupt wirkt):
1. **Abdunkeln:** Ab **Sekunde 9** des Videos legt der Code einen **Schleier** über das Bild, der von
   durchsichtig auf voll deckend blendet — **Zielfarbe = Portal-Hintergrund `#080815`** (nicht reines
   Schwarz!). Dauer **~1–1,5 Sek.** (Richtwert, **im Code fein justierbar**, „so dass es funktional passt").
   **Wichtig:** Der Schleier muss **spätestens mit dem Video-Ende (Sek. 10) voll deckend** sein, sonst
   „geht das Video aus", bevor der Schleier zu ist → sichtbarer Ruck. Also z. B. 9,0 starten, bei 10,0 voll.
2. **DANN Portal öffnen:** Aus diesem dunklen `#080815` heraus erscheint die Portal-Seite mit ihrer
   **gestaffelten Einblende** (im Code bereits angelegt, s. u.). Erst abdunkeln, dann öffnen — nicht gleichzeitig.

### Portal-Seite: „Aufleuchten"-Wunsch + was schon im Code steckt (aus `index.html` gelesen, 13. Juli)
- **Erlaubnis (Ronny, 13. Juli):** Die Portal-Seite darf für das **Animierte** angefasst werden — solange
  **Layout, Design, Farben, Schriften, Hintergrund unverändert** bleiben. Nur „Elemente erscheinen sanfter",
  kein verändertes Aussehen. (Plus die ohnehin erlaubte Ausnahme: Portal-Überschriften evtl. umbenennen.)
- **Schon vorhanden im Code:** Das Menü (`#menu-screen`) blendet per Opacity/Transform ein; die vier
  Portale haben eine **gestaffelte Einblende** (`portalEnter`, Delays 0.9s/1.1s/1.3s/1.5s) + sanftes
  Schweben (`portalFloat`). Es gibt ein fertiges **Licht-Aufblitzen** (`#bloom`: warmes Weiß → Gold →
  Violett) — nutzbar u. a. als Lichtblitz für **Naht 1**. → Ronnys „Tore erleuchten langsam" ist **größtenteils
  schon da**; der Code-Watson muss nur **verfeinern + an den Video-Übergang anschließen**, nicht neu bauen.

### Echte Farbwerte der Portal-Seite (aus `index.html`, für Prompts & Code)
- **Hintergrund (dunkel):** radial `#080815` (Mitte) → `#010103` (Rand); Grundton `#030308`.
- **Holo-Gitter-Linien:** `rgb(130,175,245)` bei nur **~5 %** Deckkraft (sehr zart).
- **Gold:** `#d4af37` · **Violett:** `#b19ffb` (= `rgb(177,159,251)`).
- **Merke:** Die Portal-Seite ist **sehr dunkel** (fast schwarz-blau), **nicht** hellblau. Das Video muss
  also in dieses dunkle `#080815` münden — passt perfekt zum „dunkel ausklingen".

### Referenz-Dateien (im Projekt hochgeladen)
- **`Video_1.png`** = Endbild von Video 1 = **Startbild von Video 2** (blaues Quanten-Netz).
- **`schwarzes_Ende.png`** = schwarzes Konzept-Endbild. **Nicht** mehr als Firefly-Endbild benutzt
  (s. o.), bleibt als Referenz für den Code-Schwarz-Schleier.
- **`Page_Seite_2_.png`** = Screenshot der Portal-Seite (Farb-/Stimmungs-Vorlage, **nicht** exakte Schablone).
- **`index.html`** wurde am 13. Juli in den Chat hochgeladen und **gelesen** → echte Portal-Farbwerte + vorhandene
  Animationen bekannt (s. o.). (Der laufende Code selbst ist im Chat nicht „live" sichtbar, nur diese eine Kopie.)

### Dateigröße (für später notiert)
Ein Video liegt bei „normaler" Auflösung bei ca. **70 MB** — für Web hoch (zwei Videos ≈ 140 MB Ladelast).
**Später optimieren:** moderner Codec (H.265 / WebM), Bitrate, Länge, Auflösung. 1080p statt 4K hilft
schon. **Aufgabe für später gemerkt.**

## 5b. Frühere Code-Pläne (Schwarzes-Loch-WebGL & Platinen-Hybrid) — PAUSIERT / abgelöst

> **Status:** Durch die Video-Entscheidung (5a) **abgelöst.** Dateien und bisherige Arbeit **bleiben
> erhalten** — nichts wird gelöscht. Rückgriff möglich, falls die Video-Richtung nicht überzeugt.

Frühere Richtung (WebGL): „Flug rückwärts zum Ursprung" — Projektion (fernes Schwarzes Loch) → Tunnel →
Hardware (Platine) → zentraler Chip = Portal-Menü. Bedeutungskette **Hardware → Programm → Projektion**;
„auch wir sind nur Code auf einer 2D-Fläche" (holografisches Prinzip → Name *theholographicme*).
Ergänzung: schwarzes Loch = Weg hinein, weißes Loch = Weg hinaus → Chip als ewiger Nullpunkt.
**Bau-Stand (in `neues-intro.html`):** Teil 1 („Blick zurück auf den schrumpfenden Eingang") gebaut;
Teile 2–4 nicht. `index.html` = stabiler Live-Stand, `neues-intro.html` = Werkstatt-Preview.

## 6. Drehbuch: Portal III „Realität als Projektion" (Holodeck) — noch zu bauen

Ziel: Der Besucher *erlebt* die Simulationshypothese. Technik: Vanilla JS + Canvas, kein WebGL, mobilkompatibel.

- **Phase A – Leerer Raum:** Ankunft in einem leeren Holodeck: schwarzer Raum mit präzisem, perspektivischem **Gold-Liniengitter** (Fluchtpunkt Bildmitte), das minimal auf die Maus reagiert (Parallaxe). Text: „WAS DU REALITÄT NENNST, IST EINE PROJEKTION." Darunter klein: „Erzeuge sie."
- **Phase B – Der Befehl:** feiner goldener Kreis „PROJIZIERE" (gleiche Click-and-Hold-Mechanik wie „ERKENNE").
- **Phase C – Rendern der Realität:** bei 100 % baut sich die „Realität" ÜBER dem Gitter auf (Lichtflecken → Sterne → Nebel → Texte). Gitter verblasst, verschwindet aber **nie ganz** (Opacity ~3–5 %).
- **Phase D – Durchschauen (Kern):** bewegt der Besucher die Maus, schimmert das Gitter in einem Radius um den Cursor wieder durch. Metapher: der aufmerksame Blick entlarvt die Simulation.
- **Phase E – Inhalt:** 2–3 philosophische Fragmente, die erst beim Annähern scharf werden, z. B.:
  - „Wenn die Auflösung fein genug ist — woran erkennst du den Unterschied?"
  - „Ein Programm, das sich selbst beobachtet: Nennt man das Bewusstsein?"
  - „Vielleicht ist Mathematik keine Beschreibung der Welt. Vielleicht ist sie ihr Quellcode."
- **Bau-Reihenfolge (inkrementell, je Schritt sichtbares Ergebnis + Git-Commit):**
  1. statisches perspektivisches Gitter · 2. Maus-Parallaxe · 3. „PROJIZIERE"-Kreis · 4. Render-Übergang · 5. Durchschimmer-Effekt am Cursor · 6. Text-Fragmente

## 7. Infrastruktur (⚠️ IM UMBRUCH — Stand 9. Juli 2026, unverändert)

**Was sich geändert hat:** Die drei Domains `theholographicme.com`, `.de` und `.global` wurden **von Ronny aus Cloudflare entfernt**. Ronny hat inzwischen **5 neue Domains**; welche davon für das Projekt genutzt wird, ist **noch nicht entschieden**.

- **Cloudflare-Pages-Projekt:** **läuft weiter**, unabhängig von den gelöschten Domains. Erreichbar über die kostenlose `…pages.dev`-Adresse (im Cloudflare-Menü unter **„Workers & Pages"** → Projekt). Zum Weiterbauen/Testen reicht diese Adresse.
- **Eigene Domain zuweisen:** noch offen. Kleiner, separater Schritt für später. **Kein Zeitdruck.**
- **DMARC / E-Mail-Schutz:** Die alten `_dmarc`-TXT-Einträge hingen an den entfernten Domains. **Vermutlich mit-entfernt — zu prüfen**, sobald eine neue Domain gewählt ist.
- **Cloudflare Access (Login-Schutz „Nur ich"):** war an `theholographicme.com` gebunden. **Vermutlich mit-entfernt — zu prüfen.**
- **Cloudflare-MCP:** `.mcp.json` verbindet den Cloudflare-MCP-Server (deckt v. a. Workers/Storage ab, **nicht** DNS/Zone-Settings).

## 8. Offene Aufgaben / nächste Ziele

- **NÄCHSTER CODE-JOB: Overlay über Video 1 bauen** — Klick-und-Halte-Auslöser in der Mitte + Gravitationslinsen-Effekt aufs Netz + Lade-Logik, die bei 100 % Video 2 startet. Kann sofort beginnen (Video 1 ist fertig). Inkrementell, je Schritt Git-Commit.
- **Video 1 ins GitHub hochladen** und in `index.html` als `<video>` einbinden (stumm, Autoplay-Loop).
- **Video 2 (Kling-3.0-Netz) sichern** (`netz_kling_final.mp4`) → in `index.html` als Auslöse-Video einbinden → **Naht 1** (Lichtblitz, `#bloom` vorhanden) + **Naht 2** (Schleier ab Sek. 9 in `#080815`, dann Portal öffnen) im Code. Video 2 ist **inhaltlich fertig** (Abschnitt 5a).
- **Portal-„Aufleuchten" verfeinern** (Abschnitt 5a): vorhandene Einblende (`portalEnter`) an den Video-Übergang anschließen; nur Animation, kein Aussehen ändern.
- **Portal III (Holodeck)** bauen — Drehbuch in Abschnitt 6.
- Inhalte für **Portale II & IV**.
- **Sound** für Video 2 (später, Firefly „Generate sound effects").
- **Video-Dateigröße optimieren** (Codec/Bitrate/Länge; Abschnitt 5a).
- **Domain-Entscheidung:** eine der 5 neuen Domains auswählen und dem Pages-Projekt zuweisen.
- **Infrastruktur prüfen** (Abschnitt 7): DMARC weg? Access-Schutz weg? Nach Domain-Wahl klären.
- Optional: JavaScript aus `index.html` in eine eigene `script.js` auslagern.

## 9. Changelog

- **13. Juli 2026 (Korrektur):** **Naht-2-Widerspruch bereinigt.** Der Überblick „Die zwei Nähte" sagte fälschlich, Video 2 **ende von selbst in reinem Schwarz** (Code-Schleier nur als Notfall in der letzten Sekunde). Richtig ist die finale Fassung: Das Video klingt **nicht** schwarz aus; **der Code dunkelt ab Sekunde 9** in die Portalfarbe `#080815` ab (voll deckend spätestens bei Sek. 10), dann Portal. Überblick auf diese Fassung nachgezogen. Auch die veraltete „auf das Wurmloch zu"-Beschreibung dort korrigiert (Video 2 ist **kein** Wurmloch).
- **13. Juli 2026 (Abend):** **Video 2 GEFUNDEN.** Wurmloch verworfen (kein Modell schafft die exakte
  Schlauch-Form zuverlässig — Striche/Ringe/Warp; Abzweigungen nicht in einem Clip machbar → Grenze der
  KI-Video-Modelle bei *exakter Geometrie*). Neuer Flug (**Kling 3.0**): **atmendes Quanten-Netz → aufsteigende
  geometrische Figur (spitz, „Fontäne") → Sterne verblassen**, 10 Sek., ab Sek. 9 Ausklang. Passt zur Design-
  Identität. **`index.html` gelesen** → echte Portal-Farben (`#080815`/`#010103`, Gitter `rgb(130,175,245)`@5%,
  Gold `#d4af37`, Violett `#b19ffb`) + vorhandene Animationen (`portalEnter` gestaffelt, `#bloom` Lichtblitz).
  **Naht 2 final:** Code-Schleier ab **Sek. 9** → Zielfarbe **`#080815`**, ~1–1,5 Sek. (im Code justierbar),
  **spätestens bei Sek. 10 voll deckend**; **danach** Portal öffnen (nacheinander, nicht gleichzeitig).
  Portal-Seite darf fürs **Animierte** angefasst werden (Layout/Design/Farben/Schriften/Hintergrund bleiben).
  Modell-Praxis: Ray HDR (schön, aber 5 Sek. + dunkelt Startbild ab + teuer 1800 Cr.), Ray normal (9 Sek., 900 Cr.,
  kein Seed-Feld), Veo (Seed änderbar, teurer), Kling (günstig, Treffer). Farbwerte statt „heller" via Adobe-Stock-KI.

- **13. Juli 2026:** **Startseite als INTERAKTIVE Zwei-Video-Architektur festgelegt** (Abschnitt 5a) — Gegenteil des still ablaufenden Videos vom 11. Juli. Kette: **Video 1 (Ambient-Loop, stumm, fertig & gekauft) → Overlay mit Klick-und-Halte-Auslöser + Gravitationslinse (Code) → Video 2 (Flug, einmalig, endet schwarz, Ton erlaubt) → Portal-Seite aus Schwarz.** Auslöser bewusst als **Ritual** (Klick-und-Halten in der Mitte). **Naht 1** = Frame-Matching (Firefly-Startbild = Ruhebild) + Code-Lichtblitz; **Naht 2** = Schwarz-Ausklang + Code-Schwarz-Schleier. **Schriftzug** „Cognizance World" nicht ins Video, sondern als Code-Overlay (evtl. Seite 2). **Firefly Video 2:** Modell **Veo 3.1** (Adobe-Modell schwächer; Alternativen Kling 3.0 Omni, Runway Gen 4.5; Sora 2 meiden), **Startbild `Video_1.png`, kein Endbild** (sonst Kamera-Sperre), **16:9 / 1080p / 8 Sek.** **Farbe:** durchgehend harmonisch blau → gold/violett → schwarz. **Video 2 v1 generiert:** Netz + Universum gut; Wurmloch/Sog/Abzweigungen noch offen → nachgeschärfter Prompt (Wurmloch+Sog zuerst, Abzweigungen später, evtl. nicht in einem Clip lösbar). **Recherche:** Firefly First/Last-Frame bestätigt; Endbild sperrt Kamerabewegung; Modell-Vergleich 2026. **Orano** = Echtzeit-Code-Erlebnis (kein Video). **Dateigröße** ~70 MB/Video → später optimieren.
- **11. Juli 2026:** Grundsatz-Entscheidung: Startseite komplett neu als eingebettetes Firefly-Video (löst WebGL-Schwarze-Loch-Intro ab; Code-Platinen-Hybrid pausiert, Dateien bleiben). Recherche geklärt: „Video → lesbarer Code" geht nicht; Lottie nur für Vektor/Linien; After-Effects-Video nicht via Bodymovin in Code wandelbar. Naht-Lösung: Video endet schwarz → Portal-Seite aus Schwarz.
- **9. Juli 2026:** Hybrid-Umbau (Code-Platine) begonnen in `neues-intro.html`; Teil 1 gebaut. Unsterblichkeits-Kreislauf ergänzt. *(Seit 11./13. Juli pausiert.)*
- **9. Juli 2026:** Vision fürs „Innere" + Ende (Platine/Chip); Arbeitsregel: kein „schnell", nur Qualität, immer erst erklären und auf „Go" warten.
- **9. Juli 2026:** Navigations-Buttons + Platzhalter-Seiten für Tore II–IV gebaut.
- **9. Juli 2026:** WebGL-Schwarze-Loch-Intro fertig & in `index.html` integriert (später abgelöst).
- **9. Juli 2026:** Alle drei `theholographicme`-Domains aus Cloudflare entfernt; 5 neue Domains, Auswahl offen; Infrastruktur „im Umbruch".
- *(früher)* Haupt-Domain cognizance.world → theholographicme.com; Auge-des-Beobachters-Intro; Wurmloch (4D-Tesserakt); DMARC repariert; Website privat via Access.
