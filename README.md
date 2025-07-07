# GameShop – Projektdokumentation

## Inhaltsverzeichnis

1.  [Intro](#intro)
2.  [Planung & Vorbereitung](#planung--vorbereitung)
3.  [Erstellung der Wireframes](#erstellung-der-wireframes)
4.  [Integration von KI](#integration-von-ki)
5.  [Technische Herausforderungen](#technische-herausforderungen)
6.  [Design & Layout-Entwicklung](#design--layout-entwicklung)
7.  [Zusätzliche Features](#zusätzliche-features)
8.  [Reflexion & Verbesserungspotential](#reflexion--verbesserungspotential)

---

## 1. Intro

Für unser Abschlussprojekt hatten wir 3 Möglichkeiten: 1. ein Blog, 2. ein Portfolio und 3. ein Webshop. Ich habe mich für einen Webshop entschieden, da es meiner Meinung nach einfacher zu erstellen ist man kann alles verkaufen, es sollte nur ein gewisses Thema dahinter liegen. Und ich hatte schon eine grobe Idee was ich machen wollte, nämlich da ich in meiner Freizeit game, dachte ich mir, mache ich doch eine Plattform worauf man Spiele kaufen kann.

Dazu nahm ich Instant Gaming (https://www.instant-gaming.com) eine Seite wo man für billig Spiele kaufen kann als Vorlage. Die Idee von GameShop gefällt mir super, da viele Spieler immer auf der Suche nach den neuesten Spielen und guten Angeboten sind. Bei GameShop kann man auch die Spiele nach Kategorien filtern um Games zu finden, die eher zu seinem Geschmack passen. Ausserdem habe ich auch noch detaillierte Produktseiten mit spezifischen Informationen zu jedem Spiel hinzugefügt, falls man ein besseres Verständnis zu dem Game haben will.

---

## 2. Planung & Vorbereitung

1.  **Wireframes erstellen**
    Ich hatte schon bisschen Zeitdruck, da ich mich nicht entscheiden konnte wie das ganze Design aussehen sollte und darum eher später mit dem Coden angefangen habe. Am Anfang habe ich zuerst mit Figma ein Wireframe erstellt wie das ganze ungefähr aussehen sollte auf Desktop und Handy.

2.  **Ordnerstruktur erstellen**
    Zunächst wollte ich eine einfache Struktur mit separaten Ordnern für CSS, JavaScript und Images.

3.  **Dateien erstellen**
    Basierend auf dem Projekt wusste ich, dass mindestens 4 HTML-Dateien benötigt werden (Startseite, Produktübersicht, Produktdetails und Kontakt). Zusätzlich brauchte ich eine umfassende CSS-Datei für das komplette Styling.

4.  **Grundstruktur der HTML-Dateien**
    Die Verknüpfung zwischen den Dateien wurde mit einem Header und der grundlegenden Navigation hergestellt. Hier habe ich schon früh auf eine konsistente Struktur geachtet.

5.  **Erneutes Überprüfen des Projektauftrags**
    Um nichts zu vergessen habe ich immer die Checkliste angeschaut zur Überprüfung, dass ich wirklich alles habe. Besonders wichtig war mir, dass ich alle Anforderungen wie Grid-Layout, Formulare und responsive Design erfülle.

6.  **Implementierung des Designs**
    Hier kam der schwierige Teil: Design. Wie ich auf das Design gekommen bin, ist durch Schauen anderer Seiten wie Instant Gaming, und da mir das Design eigentlich gut gefallen hat, versuchte ich dies zu kopieren und habe noch ein moderneres Gaming-Design hinzugefügt.

---

## 3. Erstellung der Wireframes

Die Wireframes wurden in **Figma** erstellt und zeigen die grundlegende Struktur für Desktop und Mobile.

**Figma-Link:** [https://www.figma.com/design/MDyKfLJWdd5E9tv4jxooNb/Webshop-Wireframe?node-id=0-1&t=sEsS6sIzAjcOrSu6-1](https://www.figma.com/design/MDyKfLJWdd5E9tv4jxooNb/Webshop-Wireframe?node-id=0-1&t=sEsS6sIzAjcOrSu6-1)

### Desktop Version
-   Header mit Logo und Navigation
-   Hero-Bereich mit Hauptüberschrift
-   Produktgrid mit 3-4 Spalten
-   Newsletter-Sektion
-   Footer

### Mobile Version
-   Zusammengeklappte Navigation
-   Einspaltige Produktansicht
-   Touch-optimierte Buttons
-   Responsive Formulare

---

## 4. Integration von KI

### Spezifischer Einsatz von KI

| Tool             | Einsatzgebiet                    | Beispiel                                          |
| :--------------- | :------------------------------- | :------------------------------------------------ |
| **GitHub Copilot** | Code-Vervollständigung, CSS-Styling | "Erstelle ein responsive Grid-Layout für Produktkarten" |
| **ChatGPT**      | Problemlösung, Bugfixing         | "Warum funktioniert mein CSS-Filter nicht?"       |
| **Claude**       | Content-Erstellung               | "Schreibe Produktbeschreibungen für Gaming-Titel" |

**Prozess**: Problem identifizieren -> KI um Hilfe fragen -> Vorschlag erhalten -> manuell anpassen -> testen.

### Genereller Einsatz von KI

Um ehrlich zu sein, habe ich meiner Meinung nach ein bisschen viel AI benutzt, da ich relativ spät angefangen habe mit dem Coden, da ich mir nicht sicher war wie meine ganze Seite aussehen wird und wie ich am besten umsetzen soll. Wie schon erwähnt, habe ich am meisten mit Copilot gearbeitet, da es meiner Meinung nach sehr nützlich ist es hat direkt Zugriff auf meinen Code und auch die benötigten Infos dazu, da es ja vollen Zugriff auf mein Projekt hat.

Es gab Momente wo mir AI nervig wurde, nämlich wenn ich nach Verbesserungen fragte oder irgendwas anderes das den Code veränderte gab es ein Risiko, dass es mit dem Rest des Codes nicht mehr funktioniert und ich das ganze wieder debuggen musste.

Mein Ziel ist es, in Zukunft ein bisschen weniger AI zu benutzen, da ich ja am Schluss das selber umsetzen können muss. Es ist ein neues Tool mit dem wir jetzt leben müssen, aber ich will das auch selber können und es macht mehr Spass so.

---

## 5. Technische Herausforderungen

### Der JavaScript zu CSS-only Wechsel

Einer der grössten Probleme war das Wechseln von JavaScript auf nur HTML und CSS. Ich hatte zuerst die Filter-Funktion mit Buttons und JavaScript implementiert, aber als ich danach gesehen habe, dass man 100% nur HTML und CSS benutzen darf, musste ich das natürlich ändern, was mühsam war.

Da vorhin alle meine Produkt-Infos in einem separaten JavaScript-File waren, musste ich für jedes einzelne Produkt eine HTML-Datei erstellen, was mühsam war aber nicht unmöglich. Das mit dem Filtern habe ich am Schluss mit CSS gelöst mithilfe von Radio-Buttons und CSS-Selektoren.

### Weitere Herausforderungen
-   **Responsive Design**: Besonders das Grid-Layout für verschiedene Bildschirmgrössen.
-   **CSS-only Filter**: Komplexe Selektoren für die Kategoriefilterung.
-   **Konsistente Navigation**: Zwischen allen Seiten.
-   **Performance**: Optimierung der CSS-Animationen.

---

## 6. Design & Layout-Entwicklung

### Gaming-Theme Entwicklung

Das Gaming-Theme entwickelte sich durch mehrere Iterationen:

1.  **Inspiration von Instant Gaming**: Klare Struktur und Produktfokus.
2.  **Moderne Gaming-Ästhetik**: Dunkles Theme mit Neon-Akzenten.
3.  **Animierte Elemente**: Hover-Effekte und Hintergrund-Animationen.
4.  **Spiel-spezifische Farben**: Jedes Spiel hat eigene Gradient-Farben auf den Produktkarten.

### Layout-Besonderheiten

-   **Responsive Grid**: Passt sich automatisch der Bildschirmgrösse an.
-   **Card-Design**: Moderne Produktkarten mit Hover-Effekten.
-   **Gaming-Schriftarten**: Orbitron für Headlines, Inter für Lesetext.
-   **Partikel-Animation**: Subtile Hintergrund-Effekte für Gaming-Atmosphäre.

Das meiste CSS in meinem Projekt war das Styling der verschiedenen Gaming-Elemente und Produktkarten.

---

## 7. Zusätzliche Features

1.  **CSS-only Kategoriefilter**: Ohne JavaScript implementiert.
2.  **Responsive Design**: Funktioniert auf allen Geräten.
3.  **Gaming-Animationen**: Partikel-Effekte und Hover-Animationen.
4.  **Spiel-spezifische Designs**: Individuelle Farben pro Game.
5.  **Moderne UI-Elemente**: Cards, Buttons mit Gradient-Effekten.
6.  **Newsletter-Integration**: Vollständiges Formular-Design.

---

## 8. Reflexion & Verbesserungspotential

Das ganze hat mir eigentlich recht Spass gemacht, einerseits da die Benutzung von AI erlaubt war und ich darum auf ein schöneres Design zielen konnte, und allgemein finde ich eigene Websites zu erstellen noch recht amüsant.

Es war ein sehr cooles Projekt, das viel Raum für Kreativität liess. Das Ziel war nicht, die komplexeste Website zu erstellen, sondern eine, die mir persönlich gefällt und funktional ist. Auch wenn ich im Nachhinein erkannt habe, dass ich relativ viel mit KI gearbeitet habe (hauptsächlich aufgrund von Zeitdruck und Unsicherheit beim Design), denke ich, dass ich viel aus diesem Projekt gelernt habe.

### Verbesserungspotential:
-   Weniger KI-Abhängigkeit entwickeln.
-   Bessere Zeitplanung für zukünftige Projekte.
-   Mehr eigene CSS-Experimente wagen.
-   Accessibility-Features implementieren.