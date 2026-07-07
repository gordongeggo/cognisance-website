# CLAUDE.md

**Projekt:** TheHolographicMe (früher „cognizance.world") – ein interaktives digitales
Kunstwerk über Wahrnehmung, Quantenphysik und Bewusstsein. Vanilla JS + HTML5-Canvas,
kein WebGL, mobilkompatibel; alles in `index.html`. Live über Cloudflare Pages
(Deployment automatisch bei Push zu GitHub).

👉 **Vollständige, aktuelle Projekt-Übersicht: siehe `PROJEKT-ZUSAMMENFASSUNG.md`** (Stand, Domains, Infrastruktur, Drehbücher, offene Aufgaben). Diese Datei hier ist nur die Kurzfassung.

## Über den Entwickler
Ronny ist **absoluter Anfänger**. Jeden Schritt VORHER in einfachem Deutsch erklären,
keine Fachbegriffe ohne Erklärung, Aktionen bestätigen lassen. Kleine Schritte, nach jedem
ein sichtbares Ergebnis. Git-Identität: Ronny Hammer / ronny.hammer1@icloud.com

## Design-Identität (verbindlich)
Präzise und **mathematisch statt verspielt**, exakte Geometrie, möglichst kein zufälliger
„Staub". Typografie scharf, dünn (font-weight 100–300), weit gesperrt, Titel in Großbuchstaben.
Farbwelt: Schwarz-Blau (#030308/#080815), Gold #d4af37, Violett #b19ffb, Sternenweiß.
Leitmotiv „Holodeck-Gitter": perspektivisches Liniengitter als „Struktur hinter der Realität".

## Aktueller Stand (Kurz)
Startseite mit „Auge des Beobachters" → „ERKENNE" gedrückt halten → Explosion →
geometrischer **Wurmloch-Flug mit 4D-Tesserakt** → Menü „Vier Tore der Erkenntnis" →
Kapitel I fertig (Einstein). Portale II–IV noch offen.
Live auf **theholographicme.com** (`.de`/`.global` leiten dorthin um), DMARC auf allen
dreien = `p=reject`. Seite ist per **Cloudflare Access privat** geschaltet bis zum Launch.

## Offene Aufgaben (Details in der Zusammenfassung)
- Portal III „Realität als Projektion" (Holodeck) bauen
- Inhalte für Portale II & IV
- cognizance.world aufräumen; ggf. Ordner in `TheHolographicMe` umbenennen; evtl. `script.js`
- Jeden Arbeitsschritt mit Git-Commit sichern

## Pflege
Nach jeder größeren Änderung `PROJEKT-ZUSAMMENFASSUNG.md` mit aktualisieren und committen
(sie ist Ronnys teilbarer Kontext fürs claude.ai-Projekt).
