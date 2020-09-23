# Die Übungswebsite mit Bootstrap 5  

Zugeschaut und mitgebaut ...   
Übungswebsite von https://html-und-css.de mit Bootstrap 5  

---

## 01 Bootstrap Template 
- grundlegendes Bootstrap-Template
- BootstrapCSS via BootstrapCDN 
- Eigenes CSS in `css/mein.css`
- `link`-Elemente zum CSS am Ende des `head`

---

## 02 Site-Header 
- Site-Header mit Container, Logo und Slogan 
- `header.site-header` > `div.container` 
- Utilities `pt-3` und `pb-0`
- optional: `.container` auf 960px begrenzen (Motto: "Contain the Container")

---

## 03 Site-Navigation 
- `nav.site-nav` > `div.container` 
- `.navbar` mit expand, dunkel, Schatten, sticky-top, p/m 
- Menübutton als `.navbar-toggler`
- Hauptnavigation als `.navbar-collapse` 
    - benötigt `bootstrap.min.js` 
    - via BoostrapCDN vor `</body>` einfügen

- Gestaltung der Listenelemente mit eigenem CSS 
    - in `css/mein.css`
    - Rahmenlinien für die Listenelemente 
    - sonstige Gestaltung für die Links 
    - Farbwerte mit Boostrap-Root-Variablen wie z. B. `var(--bs-light)` 

- Gestaltung der Desktop-Navi ginge zum Teil auch mit Bootstrap-Utilities 
    - `text-center`
    - `px-3` 
    - `border-left` und `border-right` 
    - `border-light` 

---

## 04 Startseite > Abschnitt "Content-Intro"  
- `main.site-content` > `section.content-intro` > `div.container` 
- H2 und Fließtext 
- einspaltiger Inhalt ist auch ohne `.row` und `.col` horizontal bündig 

---

## 05 bis 07 Startseite > Abschnitt "Infoboxen" 
- in verschiedenen Varianten 
- mit versteckter H2-Überschrift "Die Bereiche der Website" 
<!-- Frage: Kind von .row sollte immer .col sein. Gilt das auch für .sr-only-Inhalte? --> 
- die Artikel in den Spalten haben h3-Überschriften

### 05 Infoboxen klassisch 
Klassisches Bootstrap-Verhalten: 3-spaltig ab sm
- `section.infoboxen` mit `.bg-light` > `.container` 
    - h2.sr-only "Die Bereiche der Website" 
    - klassisch: 1x `.row` mit 3x `.col-sm-4` 
    - in jeder Spalte 1x `article.card` 
- Karten 
    - `div.card-body` > `h3.card-title`, `p.card-text` und `a`
    - `.card` gestalten mit Utilities `border-0` und `mb-3`

### 06 Infoboxen mit row-cols 
- Steuerung des Verhaltens zentral in `.row` 
    - `.row-cols-1` 
    - `.row-cols-sm-2` 
    - `.row-cols-md-3`
- Spalten nur mit `.col` (ohne -sm-4 etc.)


### 07 Infoboxen mit Boostrap-Icons 
Im Abschnitt `.infoboxen` 3x ein Bootstrap-SVG-Icons einbauen 
- RSS (der quadratische Rahmen drumherum wird auskommentiert, SVG ist cool)
- People-Fill 
- At 

---

## 08 Startseite > Abschnitt "Kundenstimmen" 
Mehrfach 12-Spalten in einer Zeile 
- `section.kundenstimmen` > `div.container` 
- Überschrift mit `.col-12` über die ganze Zeile 
- darunter drei Zitate 
    - xtra-small mit 3x `.col-12` 
    - small mit 2x `.col-sm-2` und 1x `.col-sm-12`
    - ab medium 

---

## 09 Site-Footer 
- `footer.site-footer` > `div.container` 
- darin eine Meta-Navigation mit `nav.navbar` 
    - die Liste `ul` wird Flex-Container 
    - Abstände rechts mit Utilities 
    - `mr-3` für den ersten Link
    - `mr-auto` beim 2. Link schiebt Link Nr. 3 nach rechts außen

---

## 10 Template mit Header, Navigation und Footer
Vorlage mit Header, Navigation, und Footer   
Ohne Inhalt

---

## 11 Startseite komplett 
Template plus Content-Abschnitte für die Startseite 
Navigationslink aktivieren
    
---

## 12 Seite News komplett 
Template plus Content-Abschnitte für die Seite News.  
Inhalte in `main.site-content` hinzufügen: 
- nur einen `div.container`, da es keine farblichen Abschnitte gibt 
- erster Abschnitt `section.col.content-intro` über ganze Breite 
- zweiter Abschitt ist zweispaltig 
    - `div.row` mit größerem Gutter `.gx-5` 
    - alle H2 als `.sr-only` 
    - Beitragsliste `section.col-md-8.beitragsliste` 
    - Linklisten als `aside.col-md-4.linklisten` 
    - Gestaltung der Artikel und Linklisten mit Bootstrap-Utilities 
- Navigationslinks aktivieren (auch auf der Startseite) 

---


--- eof --- 
