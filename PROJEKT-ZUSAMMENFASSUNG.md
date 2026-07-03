# cognizance.world — Projekt-Zusammenfassung

> Diese Datei ist als **Kontext zum Teilen** gedacht: Du kannst sie in einem
> anderen Claude-Chat oder als Wissensquelle in einem claude.ai-„Projekt"
> hochladen, damit der Gesprächspartner den Stand des Projekts kennt.
> Stand: 3. Juli 2026.

---

## Was ist das?

**cognizance.world** ist ein interaktives digitales Kunstwerk über **Wahrnehmung,
Quantenphysik und Bewusstsein**. Es ist eine einzelne Webseite, die live über
**Cloudflare Pages** läuft (Deployment automatisch bei jedem Push zu GitHub).

- **Web-Adresse:** cognizance.world (mit „z")
- **GitHub-Repository:** github.com/gordongeggo/cognisance-website (mit „s")
- **Ordner auf dem Rechner:** `cognisance-website` (mit „s")
- Die unterschiedliche Schreibweise (s/z) ist rein kosmetisch und stört nichts.

## Über den Entwickler

Ronny ist **absoluter Programmier-Anfänger**. Wichtig für jede Zusammenarbeit:
- Jeden Schritt **in einfachem Deutsch erklären, bevor** er ausgeführt wird.
- **Keine Fachbegriffe ohne Erklärung.**
- Git-Identität: Ronny Hammer / ronny.hammer1@icloud.com

## Technik

- **Vanilla JavaScript + HTML5-Canvas**, **kein** WebGL, keine Frameworks.
- **Mobilkompatibel** (funktioniert auch per Touch auf dem Handy).
- Aktuell steckt **alles in einer Datei**: `index.html` (HTML + CSS + JavaScript zusammen).
- **Farbwelt / Stil:** Dark-Tech, samtiges Schwarz-Blau, Gold (#d4af37),
  Violett (#b19ffb), Sternenweiß.

## Aktueller Ablauf der Seite (Stand jetzt)

1. **Startbildschirm:** 400 Canvas-Partikel formen bei Mausbewegung langsam ein
   „Auge des Beobachters", das dem Cursor folgt. In der Mitte der Schriftzug „ERKENNE".
2. **Aufladen:** Maustaste auf „ERKENNE" **gedrückt halten** → ein goldener Ring
   lädt sich auf.
3. **Explosion:** Bei voller Aufladung zerplatzen die Partikel.
4. **Wurmloch-Flug (~6,5 Sek.):** Ein geometrischer Tunnel aus **geraden Linien und
   durchkreuzten, rotierenden Quadraten** rast auf den Betrachter zu; die Tunnelachse
   schlängelt sich. Kurz schimmert eine **DNA-Doppelhelix** durch. In der Mitte fliegt
   ein **rotierender Tesserakt (4D-Hyperwürfel)** durch — als Andeutung der 4. Dimension,
   die wir in unserer 3D-Welt nicht direkt sehen können. Zum Ende bremst der Flug sanft ab.
5. **Austritt:** Ein weicher goldener Lichtschein.
6. **Menü „Vier Tore der Erkenntnis":** Vier schwebende Portale erscheinen gestaffelt:
   - **I. Die Illusion der Zeit** — führt zu Kapitel I (fertig; Einstein-Zitat).
   - **II. Außerirdische Intelligenz** — Inhalt folgt noch.
   - **III. Realität als Projektion** — Inhalt folgt noch.
   - **IV. Wachstum durch KI** — Inhalt folgt noch.
7. **Kapitel I** öffnet sich beim Klick langsam (4,5 Sek. Einblendung).

## Offene Aufgaben / nächste Ziele

- Inhalte für die **Portale II, III und IV** gestalten (zeigen aktuell „Dieses Tor
  öffnet sich bald …").
- Optional: den **JavaScript-Code aus `index.html` in eine eigene `script.js`
  auslagern** (nur Aufräumen, ändert nichts am Aussehen).
- Optional: den Ordner später in **`cognizance-world`** umbenennen (kontrolliert,
  wegen der GitHub-Verbindung).

## Wie das Veröffentlichen funktioniert

Änderungen an `index.html` → mit Git **committen** (Speicherpunkt) → zu **GitHub
pushen** (hochladen) → **Cloudflare Pages** baut die Seite automatisch neu
(dauert 1–2 Min.). Danach im Browser mit **Cmd + Shift + R** hart neu laden, um
die neue Version zu sehen.

## Arbeitsweise

- Die **technische Arbeit** (Code, Speichern, Hochladen) passiert in **Claude Code**,
  weil dort Zugriff auf Dateien, Terminal und GitHub besteht.
- Der **normale claude.ai-Chat** hat diesen Zugriff nicht — er eignet sich für Ideen,
  Texte und Konzept-Gespräche. Diese Zusammenfassung dient dazu, ihn auf den Stand
  zu bringen.
