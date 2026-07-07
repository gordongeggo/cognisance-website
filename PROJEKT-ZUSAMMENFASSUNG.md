# TheHolographicMe — Projekt-Übergabe & Zusammenfassung

> **Eine Datei für alles.** Dieses Dokument ist die *einzige* aktuelle Projekt-Übersicht.
> Es vereint und ersetzt die früheren Dateien `PROJEKT-ZUSAMMENFASSUNG.md` (alt) und
> `UEBERGABE-HOLODECK.md`. Du kannst es in einen anderen Claude-Chat oder als
> Wissensquelle in dein claude.ai-Projekt hochladen.
> **Stand: 7. Juli 2026.**

---

## 1. Was ist das Projekt?

Ein interaktives digitales **Kunstwerk über Wahrnehmung, Quantenphysik und Bewusstsein**.
Eine einzelne, statische Website, live über **Cloudflare Pages** (Deployment automatisch
bei jedem Push zu GitHub).

- **Neue Haupt-Adresse (live):** **theholographicme.com** (mit den Varianten `.de` und `.global`, die dorthin umleiten)
- **Früher:** cognizance.world (wird abgelöst / soll aufgeräumt werden)
- **Aktuell NICHT öffentlich:** Die Seite ist per Cloudflare Access hinter einem Login verborgen (siehe Abschnitt 7), bis der Aufbau fertig ist.
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
> Später ggf. angleichen (Entscheidung offen).

## 5. Aktueller Ablauf der Website

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

## 7. Infrastruktur (Stand 7. Juli 2026 — heute eingerichtet)

- **Domains & Weiterleitungen:** `theholographicme.com` ist die Haupt-Domain. `theholographicme.de` und `theholographicme.global` leiten per **Cloudflare Redirect Rule** (301, „Alle eingehenden Anforderungen" → `concat("https://theholographicme.com", http.request.uri.path)`) auf `.com` um. Dafür hat jede `.de`/`.global` einen **proxied Dummy-DNS-Eintrag** (A → 192.0.2.1, orange Wolke), damit der Verkehr Cloudflare erreicht.
- **DMARC (E-Mail-Schutz):** Auf **allen drei** theholographicme-Domains steht jetzt ein **TXT-Eintrag `_dmarc` = `v=DMARC1; p=reject;`** (Nur DNS). Vorher war der von IONOS importierte `_dmarc`-CNAME fälschlich „proxied" (orange) → DMARC unsichtbar. Die drei Domains nutzen **keine** E-Mail, daher `p=reject` (stärkster Schutz).
- **Privat bis Launch:** `theholographicme.com` ist durch **Cloudflare Access (Zero Trust)** geschützt. Anwendung „theholographicme.com", Richtlinie **„Nur ich"** = `ronny.hammer1@icloud.com`, Anmeldung per One-time PIN (oder „mit Cloudflare"), Sitzung 24 Std. Team-Domain: `lucky-lake-2a39.cloudflareaccess.com`. **Zum Öffentlich-Schalten: diese eine Access-Anwendung löschen.**
- **Cloudflare-MCP:** `.mcp.json` im Projekt verbindet den Cloudflare-MCP-Server (`https://mcp.cloudflare.com/mcp`). Der „Cloudflare Development Platform"-Konnektor ist autorisiert (deckt aber v. a. Workers/Storage ab, **nicht** DNS/Zone-Settings).

## 8. Offene Aufgaben / nächste Ziele

- **Portal III (Holodeck)** bauen — Drehbuch in Abschnitt 6.
- Inhalte für **Portale II & IV**.
- **Design-Abgleich:** Wurmloch ggf. an die strengere Identität anpassen (Staub?) — Entscheidung offen.
- **cognizance.world aufräumen:** IONOS-E-Mail-Adressen löschen + Domain aus Cloudflare entfernen (Website läuft ja auf `.com`).
- Optional/kosmetisch: Schreibtisch-Ordner in `TheHolographicMe` umbenennen (nur wenn keine Claude-Code-Sitzung läuft); Cloudflare-Pages-Projekt umbenennen.
- Optional: JavaScript aus `index.html` in eine eigene `script.js` auslagern.
- **Vor dem Launch:** die Cloudflare-Access-Anwendung löschen → Seite ist für alle offen.

## 9. Was sich gegenüber den alten Protokollen geändert hat (Changelog)

- Haupt-Domain **cognizance.world → theholographicme.com** (+ `.de`/`.global`-Weiterleitungen).
- Wurmloch **neu gestaltet** (geometrisch + 4D-Tesserakt statt runder Ringe/Staub-Vortex), Auge & Kapitel-Einblendung **langsamer**.
- **DMARC** auf allen drei neuen Domains repariert (p=reject).
- Website **privat** geschaltet (Cloudflare Access).
- Diese Datei **vereint** die frühere Zusammenfassung und die Holodeck-Übergabe (`UEBERGABE-HOLODECK.md` kann gelöscht werden, Inhalt ist hier integriert).
