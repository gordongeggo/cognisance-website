# TheHolographicMe — Projekt-Übergabe & Zusammenfassung

> **Eine Datei für alles.** Dieses Dokument ist die *einzige* aktuelle Projekt-Übersicht.
> Es vereint und ersetzt die früheren Dateien `PROJEKT-ZUSAMMENFASSUNG.md` (alt) und
> `UEBERGABE-HOLODECK.md`. Du kannst es in einen anderen Claude-Chat oder als
> Wissensquelle in dein claude.ai-Projekt hochladen.
> **Stand: 9. Juli 2026.**

---

## 1. Was ist das Projekt?

Ein interaktives digitales **Kunstwerk über Wahrnehmung, Quantenphysik und Bewusstsein**.
Eine einzelne, statische Website, live über **Cloudflare Pages** (Deployment automatisch
bei jedem Push zu GitHub).

- **Live-Adresse aktuell:** die kostenlose Cloudflare-Pages-Adresse `…pages.dev` (das Pages-Projekt läuft weiter, unabhängig von Domains).
- **Eigene Domain:** ⚠️ **im Umbruch** — siehe Abschnitt 7. Es ist aktuell **keine** eigene Domain zugewiesen.
- **Früher:** cognizance.world (abgelöst) und danach theholographicme.com (siehe Changelog / Abschnitt 7).
- **GitHub:** github.com/gordongeggo/cognisance-website · **Ordner:** `cognisance-website` (die „s/z"-Schreibweise ist rein kosmetisch)

## 2. Über den Entwickler & Arbeitsweise (WICHTIG)

**Ronny ist absoluter Programmier-Anfänger.** Für jede Zusammenarbeit gilt:
- Jeden Schritt **VORHER in einfachem Deutsch erklären**, keine Fachbegriffe ohne Erklärung, Aktionen bestätigen lassen.
- **Kleine Schritte**, nach jedem ein sichtbares Ergebnis.
- Jede Änderung mit **Git-Commit** sichern.
- **Git-Identität:** Ronny Hammer / ronny.hammer1@icloud.com

**Veröffentlichen:** Änderung an `index.html` → committen → zu GitHub pushen →
Cloudflare Pages baut automatisch neu (1–2 Min.) → im Browser mit **Cmd+Shift+R** hart neu laden.

**Werkzeug-Aufteilung:** Die technische Arbeit (Code, Git, Cloudflare) passiert in **Claude Code**.
Der normale claude.ai-Chat hat keinen Datei-Zugriff – dafür ist genau dieses Dokument da.

## 3. Technik

- **Vanilla JavaScript + HTML5-Canvas**, **kein** WebGL, keine Frameworks, `requestAnimationFrame`, mobilkompatibel.
- Aktuell steckt **alles in einer Datei**: `index.html` (HTML + CSS + JavaScript zusammen).
- **Farbwelt:** samtiges Schwarz-Blau (#030308 / #080815), Gold **#d4af37**, Violett **#b19ffb**, Sternenweiß.

## 4. Verbindliche Design-Identität (gilt für ALLE Seiten)

Das Menü nach dem Wurmloch und die Kapitel-I-Seite definieren die visuelle Identität:
- **Präzise und mathematisch statt verspielt.** Exakte Geometrie, klare Konstruktion. Möglichst **kein zufälliger „Staub"**, keine wolkige Verspieltheit.
- **Typografie:** scharf, dünn (font-weight 100–300), weit gesperrt, Großbuchstaben für Titel.
- **Leitmotiv „Holodeck-Gitter"** (Star-Trek-inspiriert): ein leeres, perspektivisches Liniengitter als „Struktur hinter der Realität". Die sichtbare Welt ist nur eine Projektion darüber; wer genau hinschaut, sieht das Gitter durchschimmern.
- Optionale Idee: Bei Seitenwechseln blitzt kurz das nackte Gitter auf, bevor sich die neue „Realität" aufbaut.

> ⚠️ **Offener Abgleich:** Das aktuelle Wurmloch enthält noch „Staub"-Partikel und wurde
> teils „verspielter" gemacht – das widerspricht leicht der obigen strengeren Linie.
> Später ggf. angleichen (Entscheidung offen). **Hinweis:** Dieser Punkt wird durch den
> geplanten Intro-Umbau (Abschnitt 5a) ohnehin berührt.

## 5. Aktueller Ablauf der Website (Ist-Zustand — das läuft heute wirklich)

1. **Startbildschirm:** 400 Canvas-Partikel formen bei Mausbewegung **langsam** ein „Auge des Beobachters". Schriftzug „ERKENNE".
2. **Aufladen:** Maustaste auf „ERKENNE" gedrückt halten → goldener Ring lädt sich auf.
3. **Explosion** der Partikel.
4. **Wurmloch-Flug (~6,5 Sek.):** geometrischer Tunnel aus **geraden Linien und durchkreuzten, rotierenden Quadraten**; die Achse schlängelt sich. Kurz schimmert eine **DNA-Doppelhelix** durch. In der Mitte fliegt ein **rotierender Tesserakt (4D-Hyperwürfel)** durch. Der Flug bremst sanft ab.
5. **Austritt:** weicher goldener Lichtschein.
6. **Menü „Vier Tore der Erkenntnis"** – vier Portale erscheinen gestaffelt:
   - **I. Die Illusion der Zeit** → Kapitel I fertig (Einstein-Zitat), öffnet sich langsam (4,5 Sek.)
   - **II. Außerirdische Intelligenz** → Inhalt folgt
   - **III. Realität als Projektion** → Inhalt folgt (Drehbuch siehe Abschnitt 6)
   - **IV. Wachstum durch KI** → Inhalt folgt

## 5a. GEPLANTER Umbau des Intros: „Flug durchs Schwarze Loch" (noch NICHT gebaut)

> **Status:** Vision steht, ein Prompt für Claude Code ist vorbereitet. **Noch nichts umgesetzt,
> noch nichts technisch geprüft.** Ersetzt nach Fertigstellung die Schritte 1–5 aus Abschnitt 5
> (Auge → Aufladen → Explosion → bisheriges Wurmloch). Das **Portal-Menü (Schritt 6) bleibt** und ist das Endziel.

**Grundlage:** Fünf Referenzbilder (`1`–`5`) liegen im Schreibtisch-Ordner. Die Zahlen geben die grobe Reihenfolge vor. Diese Bilder sind nur in **Claude Code** sichtbar (der claude.ai-Chat sieht sie nicht).

**Geplanter Ablauf:**
1. Man kommt auf die Seite und sieht in der **Ferne ein Schwarzes Loch** (Bild 1).
2. Das Loch **reagiert auf die Maus** (zwei Zonen): weit weg nur sanfte Drehung + leichte Anziehung Richtung Cursor; kommt der Cursor **nah genug ans Zentrum**, kippt es → der Sog übernimmt, der Flug startet **von selbst**, kein Entkommen mehr. (Kein Klick nötig — reine Nähe löst aus.)
3. **Flug in den Trichter** (Bilder 2–3).
4. Zwischendurch das **Konstrukt von außen** (Bild 4).
5. **Projektion** (Bild 5): Das Schwarze Loch trägt sämtliche Informationen des Universums und projiziert sie auf eine 2D-Fläche (**holografisches Prinzip** — passt zum Namen theholographicme).
6. Bild 5 steht zunächst **schräg** im Raum → dreht sich **gerade** und füllt den Bildschirm → **diese Fläche IST das Portal-Menü (Seite 2)**. Übergang nahtlos.

**Verbindliche Vorgaben:** Farbwelt und Typografie der bestehenden Seiten bleiben (siehe Abschnitt 3 + 4); die Bilder müssen farblich in genau diesen Stil gewandelt werden. Technik wie bisher (Vanilla JS + Canvas, kein WebGL, mobilkompatibel).

## 6. Drehbuch: Portal III „Realität als Projektion" (Holodeck) — noch zu bauen

Ziel: Der Besucher *erlebt* die Simulationshypothese. Technik: Vanilla JS + Canvas, kein WebGL, mobilkompatibel.

- **Phase A – Leerer Raum:** Ankunft in einem leeren Holodeck: schwarzer Raum mit präzisem, perspektivischem **Gold-Liniengitter** (Boden/Wände/Decke fluchten in die Tiefe, Fluchtpunkt Bildmitte), das minimal auf die Maus reagiert (Parallaxe). Text: „WAS DU REALITÄT NENNST, IST EINE PROJEKTION." Darunter klein: „Erzeuge sie."
- **Phase B – Der Befehl:** feiner goldener Kreis „PROJIZIERE" (gleiche Click-and-Hold-Mechanik wie „ERKENNE").
- **Phase C – Rendern der Realität:** bei 100 % baut sich die „Realität" ÜBER dem Gitter auf (Lichtflecken → Sterne → Nebel → Texte). Gitter verblasst, verschwindet aber **nie ganz** (Opacity ~3–5 %).
- **Phase D – Durchschauen (Kern):** bewegt der Besucher die Maus, schimmert das Gitter in einem Radius um den Cursor wieder durch (Projektion wird dort halbtransparent). Auf dem Handy um die Berührung. Metapher: der aufmerksame Blick entlarvt die Simulation.
- **Phase E – Inhalt:** 2–3 philosophische Fragmente, die erst beim Annähern scharf werden, z. B.:
  - „Wenn die Auflösung fein genug ist — woran erkennst du den Unterschied?"
  - „Ein Programm, das sich selbst beobachtet: Nennt man das Bewusstsein?"
  - „Vielleicht ist Mathematik keine Beschreibung der Welt. Vielleicht ist sie ihr Quellcode."
- **Bau-Reihenfolge (inkrementell, je Schritt sichtbares Ergebnis + Git-Commit):**
  1. statisches perspektivisches Gitter · 2. Maus-Parallaxe · 3. „PROJIZIERE"-Kreis (von Startseite) · 4. Render-Übergang · 5. Durchschimmer-Effekt am Cursor · 6. Text-Fragmente

## 7. Infrastruktur (⚠️ IM UMBRUCH — Stand 9. Juli 2026)

**Was sich geändert hat:** Die drei Domains `theholographicme.com`, `.de` und `.global` wurden **von Ronny aus Cloudflare entfernt** (`.de`/`.global` hatten per Redirect auf `.com` umgeleitet). Ronny hat inzwischen **5 neue Domains**; welche davon für das Projekt genutzt wird, ist **noch nicht entschieden**.

- **Cloudflare-Pages-Projekt:** **läuft weiter** und ist unabhängig von den gelöschten Domains. Die Seite ist weiterhin über die kostenlose `…pages.dev`-Adresse erreichbar (im Cloudflare-Menü unter **„Workers & Pages"** → Projekt). Zum Weiterbauen/Testen reicht diese Adresse; eine eigene Domain ist dafür **nicht** nötig.
- **Eigene Domain zuweisen:** noch offen. Kleiner, separater Schritt für später (neue Domain im Pages-Projekt als „Custom Domain" hinterlegen). **Kein Zeitdruck.**
- **DMARC / E-Mail-Schutz:** Die alten `_dmarc`-TXT-Einträge hingen an den entfernten Domains. **Vermutlich mit-entfernt — zu prüfen**, sobald eine neue Domain gewählt ist. (Nicht als erledigt annehmen.)
- **Cloudflare Access (Login-Schutz „Nur ich"):** war an `theholographicme.com` gebunden. **Vermutlich mit-entfernt — zu prüfen.** Falls die `…pages.dev`-Adresse ohne Login erreichbar ist, ist der Schutz weg; falls noch nach PIN gefragt wird, besteht er teilweise fort. (Ronny kommt aktuell ohne PIN drauf — evtl. aber nur, weil er bei Cloudflare eingeloggt ist. Unklar, daher: prüfen.)
- **Cloudflare-MCP:** `.mcp.json` im Projekt verbindet den Cloudflare-MCP-Server. Der „Cloudflare Development Platform"-Konnektor deckt v. a. Workers/Storage ab, **nicht** DNS/Zone-Settings.

## 8. Offene Aufgaben / nächste Ziele

- **Intro-Umbau „Schwarzes Loch"** (Abschnitt 5a) — Prompt liegt bereit, Claude Code soll zuerst **Feedback** geben, dann bauen.
- **Portal III (Holodeck)** bauen — Drehbuch in Abschnitt 6.
- Inhalte für **Portale II & IV**.
- **Domain-Entscheidung:** eine der 5 neuen Domains auswählen und dem Pages-Projekt zuweisen.
- **Infrastruktur prüfen** (Abschnitt 7): Ist DMARC weg? Ist der Access-Schutz weg? Status nach Domain-Wahl klären.
- **Design-Abgleich:** „Staub" im bisherigen Wurmloch — wird durch den Intro-Umbau ohnehin berührt.
- Optional: JavaScript aus `index.html` in eine eigene `script.js` auslagern.

## 9. Was sich gegenüber dem letzten Stand geändert hat (Changelog)

- **9. Juli 2026:** Alle drei `theholographicme`-Domains aus Cloudflare **entfernt**; 5 neue Domains vorhanden, Auswahl offen. Infrastruktur-Abschnitt (7) auf „im Umbruch" gesetzt; DMARC- und Access-Status als **zu prüfen** markiert (nicht mehr als erledigt behauptet). Live-Zugang läuft aktuell über die `…pages.dev`-Adresse.
- **9. Juli 2026:** Neuer **Intro-Plan „Flug durchs Schwarze Loch"** als Abschnitt 5a aufgenommen (geplant, noch nicht gebaut). Ersetzt nach Fertigstellung Schritte 1–5 des bisherigen Ablaufs; Portal-Menü bleibt Endziel.
- *(früher)* Haupt-Domain cognizance.world → theholographicme.com (+ `.de`/`.global`); Wurmloch geometrisch neu gestaltet (4D-Tesserakt); Auge & Kapitel-Einblendung langsamer; DMARC repariert; Website privat via Access. Diese Datei vereint frühere Zusammenfassung + Holodeck-Übergabe.
