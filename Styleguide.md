# GameShop Styleguide

## 1. Farbpalette

Definiert als CSS-Custom-Properties im `:root`-Selektor:

-   **--primary-color:** `#6366f1` (Indigo - Hauptfarbe)
-   **--primary-dark:** `#4f46e5` (Dunkles Indigo)
-   **--secondary-color:** `#f59e0b` (Orange - Akzent)
-   **--accent-color:** `#10b981` (Grün - Akzent)

### Hintergrundfarben
-   **--bg-dark:** `#0f172a` (Dunkler Seitenhintergrund)
-   **--bg-card:** `#1e293b` (Hintergrund für Karten und Formulare)

### Textfarben
-   **--text-primary:** `#f8fafc` (Haupttextfarbe)
-   **--text-secondary:** `#cbd5e1` (Sekundäre Textfarbe)
-   **--text-muted:** `#64748b` (Gedämpfte Textfarbe)

### Rahmen & Schatten
-   **--border-color:** `#334155` (Rahmenfarbe)
-   **--shadow-primary:** `rgba(99, 102, 241, 0.2)` (Schatten für primäre Elemente)
-   **--shadow-card:** `rgba(0, 0, 0, 0.4)` (Schatten für Karten)

### Farbverläufe
-   **--gradient-primary:** `linear-gradient(135deg, #6366f1, #4f46e5)`
-   **--gradient-accent:** `linear-gradient(135deg, #f59e0b, #10b981)`

### Spiel-spezifische Bild-Hintergründe
Diese werden für fehlende Bilder in den Produktkarten verwendet:
-   **Witcher:** `linear-gradient(135deg, #8B5A3C, #D4AF37)`
-   **Elden Ring:** `linear-gradient(135deg, #2D1B69, #F7D794)`
-   **Cyberpunk:** `linear-gradient(135deg, #FF0080, #00FFFF)`
-   **God of War:** `linear-gradient(135deg, #8B0000, #FFD700)`
-   **Hogwarts Legacy:** `linear-gradient(135deg, #740001, #D3A625)`
-   **Halo Infinite:** `linear-gradient(135deg, #0F4C75, #3282B8)`
-   **Balatro:** `linear-gradient(135deg, #FF4500, #FFD700)`
-   **Battlefront 2:** `linear-gradient(135deg, #0A0A0A, #444444)`
-   **Celeste:** `linear-gradient(135deg, #4B0082, #8A2BE2)`
-   **Cuphead:** `linear-gradient(135deg, #8B0000, #FF6347)`
-   **Dark Souls 3:** `linear-gradient(135deg, #2F4F4F, #696969)`
-   **Dead Cells:** `linear-gradient(135deg, #006400, #3CB371)`
-   **Geometry Dash:** `linear-gradient(135deg, #FFD700, #FF8C00)`
-   **Hollow Knight:** `linear-gradient(135deg, #2F4F4F, #4682B4)`
-   **Nine Sols:** `linear-gradient(135deg, #6A5ACD, #483D8B)`
-   **Sea of Thieves:** `linear-gradient(135deg, #008080, #20B2AA)`
-   **Binding of Isaac:** `linear-gradient(135deg, #A52A2A, #8B0000)`
-   **Anno 1800:** `linear-gradient(135deg, #4682B4, #5F9EA0)`

---

## 2. Typografie

### Schriftarten
-   **Inter:** `font-family: 'Inter', sans-serif;` (Für Fliesstext, Buttons, Preise, etc.)
-   **Orbitron:** `font-family: 'Orbitron', monospace;` (Für Logo, Überschriften)

### Schriftgrößen & Gewichte
-   **Logo:** `font-size: 2rem; font-weight: 900;`
-   **H1 (Hero):** `font-size: 3rem; font-weight: 700;` (Farbverlauf)
-   **H1 (Kontakt/Produktdetails):** `font-size: 2.5rem; font-weight: 700;` (Farbverlauf)
-   **H2 (Featured Games/Newsletter):** `font-size: 1.2rem; font-weight: 400; text-transform: uppercase; letter-spacing: 2px;`
-   **H3 (Produkttitel):** `font-size: 1.2rem; font-weight: 600;`
-   **Preise:** `font-size: 1.4rem; font-weight: 700;`
-   **Body Text:** `font-size: 1rem; line-height: 1.6;`

---

## 3. Layout & Grid

### Globale Einstellungen
-   `box-sizing: border-box;` für alle Elemente.
-   `min-height: 100vh; display: flex; flex-direction: column;` für Footer am Ende der Seite.

### Hauptcontainer
-   `max-width: 1400px; margin: 0 auto; padding: 0 2rem;` für zentrale Inhalte.

### Produkt-Grid (`.product-grid`)
-   `display: grid;`
-   `grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));`
-   `gap: 2rem;`
-   `max-width: 1400px; margin: 0 auto;`

### Produktdetail-Seite (`.product-detail`)
-   `display: grid;`
-   `grid-template-columns: 1fr 1fr;`
-   `gap: 3rem;`
-   `max-width: 1200px; margin: 0 auto;`

### Footer-Layout (`.footer-content`)
-   `display: grid;`
-   `grid-template-columns: 2fr 2fr 1fr;`
-   `gap: 2rem;`
-   `max-width: 1200px; margin: 0 auto; padding: 0 2rem;`

---

## 4. Komponenten

### Header
-   `background: rgba(15, 23, 42, 0.95);` mit `backdrop-filter: blur(10px);`
-   `position: sticky; top: 0; z-index: 100;`
-   `box-shadow: 0 4px 20px rgba(0, 0, 0, 0.2);`

### Navigationslinks
-   `color: var(--text-secondary); font-weight: 500;`
-   `padding: 0.5rem 1rem; border-radius: 8px;`
-   **Hover:** `color: var(--text-primary); background: rgba(99, 102, 241, 0.1); transform: translateY(-2px);`

### Produktkarten (`.product-card`)
-   `background: var(--bg-card);`
-   `border: 1px solid var(--border-color); border-radius: 20px;`
-   `box-shadow: 0 4px 20px rgba(0, 0, 0, 0.2);`
-   `height: 280px; object-fit: cover;` für Bilder.
-   **Hover:** `transform: translateY(-10px); border-color: var(--primary-color); box-shadow: 0 20px 40px var(--shadow-card);`

### Kategorie-Buttons (`.category-button`)
-   `background: var(--bg-card); border: 1px solid var(--border-color); border-radius: 16px;`
-   `padding: 1rem 2rem; color: var(--text-secondary); font-weight: 600;`
-   **Active/Checked:** `background: var(--primary-color); color: var(--text-primary); box-shadow: 0 8px 25px var(--shadow-primary);`

### Formular-Elemente (`input`, `select`, `textarea`, `button`)
-   `background: var(--bg-card); border: 1px solid var(--border-color); border-radius: 12px;`
-   `padding: 1rem; color: var(--text-primary); width: 100%;`
-   **Fokus:** `outline: none; border-color: var(--primary-color); box-shadow: 0 0 0 3px var(--shadow-primary);`

### Buttons (`button` generell)
-   `background: var(--gradient-primary); color: white; font-weight: 600;`
-   `border: none; min-width: 150px; width: auto;`
-   **Hover:** `transform: translateY(-2px); box-shadow: 0 10px 30px var(--shadow-primary);`

---

## 5. Animationen & Effekte

### Globale Hintergrund-Animationen
-   **body::before (Nebelfelder):** `background: radial-gradient(...)` mit `animation: backgroundNebula 30s linear infinite alternate;` (Sanfte Verschiebung farbiger Lichtpunkte im Hintergrund).
-   **body::after (Digitaler Staub/Sterne):** `background-image: radial-gradient(...)` mit `animation: digitalDust 45s linear infinite;` (Kleine, subtile Punkte, die sich langsam bewegen).

### Header & Logo
-   **Header::after (Neon-Linie):** `background: linear-gradient(...)` mit `animation: neonPulse 4s ease-in-out infinite;` (Pulssierende, leuchtende Linie am unteren Rand des Headers).
-   **Logo:** `animation: logoGlow 3s ease-in-out infinite alternate;` (Sanftes Aufleuchten des Logos).

### Hero-Sektion
-   **hero::before (Gittermuster):** `background: linear-gradient(...)` mit `animation: gridMove 15s linear infinite;` (Ein sich bewegendes Gitter über dem Hero-Bereich).

### Produkt-Grid
-   **product-grid::before (Circuit Board Pattern):** `background-image: linear-gradient(...)` mit `animation: circuitPulse 5s ease-in-out infinite;` (Ein pulsierendes Schaltungsmuster hinter den Produktkarten).

### Produktkarten
-   **Initiales Erscheinen (`.product-card`):** `animation: fadeInUp 0.8s cubic-bezier(.23,1.02,.57,1.01) forwards;` (Elemente gleiten beim Laden von unten nach oben ins Bild).
-   **Hover-Effekt (`.product-card::before`):** `background: linear-gradient(...)` mit `transition: left 0.6s ease;` (Ein Lichtstrahl, der beim Darüberfahren über die Karte gleitet).

---

## 6. Responsive Design

### Haupt-Breakpoint
-   `@media (max-width: 768px)`: Für Mobile-Ansichten.

### Anpassungen (Mobile)
-   **Header:** `flex-direction: column; gap: 1rem;` (Elemente untereinander).
-   **Produkt-Grid:** `grid-template-columns: 1fr;` (Einspaltige Darstellung).
-   **Produktdetails:** `grid-template-columns: 1fr;` (Bild und Details untereinander).
-   **Hero H1:** `font-size: 2rem;` (Kleinere Schrift).
-   **Footer-Inhalt:** `grid-template-columns: 1fr; text-align: center;` (Elemente untereinander, zentriert).
-   **Footer Links & Social Icons:** `justify-content: center;` (Zentrierte Ausrichtung).