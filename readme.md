# Bootstrap 5 und die Übungswebsite 

Übungswebsite von [https://html-und-css.de] mit Bootstrap 5 nachbauen 

In den einzelnen Dateien werden nur die jeweiligen Abschnitte gezeigt und gespeichert. Zusammengebaut werden die kompletten Seiten erst danach. 

Im Videokurs wird die Seite Stück für Stück aufgebaut und wächst live mit. 


## 01 Template 
- grundlegendes Bootstrap-Template
- Bootstrap via BootstrapCDN, nur CSS 
- der Link zu Bootstrap kommt *nach* dem Seitentitel 


## 02 Site-Header 
- Site-Header mit Container, Logo und Slogan 
- `header.site-header` > `div.container` 
- Utilities `pt-3` und `pb-0`
- optional: `.container` auf 960px begrenzen (Motto: "Contain the Container")


## 03 Site-Navigation 
- `nav.site-nav` > `div.container` 
- `.navbar` mit expand, dunkel, Schatten, sticky-top, p/m 
- Menübutton als `.navbar-toggler`
- Hauptnavigation als `.navbar-collapse` 
    - benötigt `bootstrap.min.js` 
    - via BoostrapCDN vor `</body>` einfügen
- Gestaltung der Listenelemente nur mit Utilities 
    - `text-center`
    - `border-left` und `border-right` 
    - `border-light` 
    - Padding mit `px-3` 


## 04 Startseite > Content-Intro 
- `main.site-content` > `section.content-intro` > `div.container` 
- einspaltiger Inhalt benötigt nicht zwingend `.row` und `.col`
- H2 und Fließtext 


## 05 bis 07 Startseite > Infoboxen 
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


## 08 Startseite > Site-Content > Kundenstimmen 
Mehrfach 12-Spalten in einer Zeile 
- `section.kundenstimmen` > `div.container` 
- Überschrift mit `.col-12` über die ganze Zeile 
- darunter drei Zitate 
    - xtra-small mit 3x `.col-12` 
    - small mit 2x `.col-sm-2` und 1x `.col-sm-12`
    - ab medium 


## 09 Site-Footer 
- `footer.site-footer` > `div.container` 
- darin eine Meta-Navigation mit `nav.navbar` 
    - die Liste `ul` wird Flex-Container 
    - Abstände rechts mit Utilities 
    - `mr-3` für den ersten Link
    - `mr-auto` beim 2. Link schiebt Link Nr. 3 nach rechts außen


## 10 Startseite komplett 
Header, Navigation, Content-Abschnitte und Footer in einer Datei.


--- eof --- 
