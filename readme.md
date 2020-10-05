# Die Übungswebsite mit Bootstrap 5  
Stand: 05.10.2020 - Bootstrap 5 alpha 2 

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
- optional: `.container` auf maximal 960px begrenzen

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

## 05 Startseite > Abschnitt "Infoboxen" 
- mit versteckter H2-Überschrift "Die Bereiche der Website" 
- die Artikel in den Spalten haben h3-Überschriften

### 05a Infoboxen mit klassischem Grid-Markup
Klassisches Bootstrap-Verhalten: 3-spaltig ab sm
- `section.infoboxen` mit `.bg-light` > `.container` 
    - h2.visually-hidden "Die Bereiche der Website" 
    - Grid 
        - 1x `.row` 
            - 3x `.col-sm-6` 
            - 3x `.col-lg-4`
            - in jeder Spalte 1x `article.card` 
- Karten 
    - `div.card-body` > `h3.card-title`, `p.card-text` und `a`
    - `.card` gestalten mit Utilities `border-0` und `mb-3`


### 05b Infoboxen mit Boostrap-Icons 
Infoboxen mit ein Bootstrap-SVG-Icons 
- RSS (der quadratische Rahmen drumherum wird auskommentiert, SVG ist cool)
- People-Fill 
- At 


---

## 06 Startseite > Abschnitt "Kundenstimmen" 
Mehrfach 12-Spalten in einer Zeile 
- `section.kundenstimmen` > `div.container` 
- Überschrift mit `.col-12` über die ganze Zeile 
- darunter drei Zitate 
    - xtra-small mit 3x `.col-12` 
    - small mit 2x `.col-sm-2` und 1x `.col-sm-12`
    - ab medium 

---

## 07 Site-Footer 
- `footer.site-footer` > `div.container` 
- darin eine Meta-Navigation mit `nav.navbar` 
    - die Liste `ul` wird Flex-Container 
    - Abstände rechts mit Utilities 
    - `mr-3` für den ersten Link
    - `ml-auto` beim schiebt Link Nr. 3 nach rechts außen
    - Link "Nach oben" mit Icon  

---

## 08 Kontaktformular  
Kontaktformular
- einspaltig (`label` immer über `input`) 
- zweispaltig responsiv (`label` über/vor `input`)

### 08a Kontaktformular 1-spaltig
wie in der Bootstrap-Doku    
DSGVO wie im Buch, Kapitel 9.8 


### 08b Kontaktformular 2-spaltig
Layout ähnlich wie beim Videokurs 
- mobil: Kontaktdaten - Kontaktformular 
- ab `sm` 
    - `label` rechtsbündig vor den Eingabefeldern 
    - DSGVO und Button mit offset-sm-2 

---

## 09 Template mit Header, Navigation und Footer
Vorlage mit Header, Navigation, und Footer   
Ohne Inhalt

---

## Startseite komplett 
Template plus Content-Abschnitte für die Startseite 
Navigationslink aktivieren
    
---

## Seite News komplett 
Template plus Content-Abschnitte für die Seite News.  
Inhalte in `main.site-content` hinzufügen: 
- nur einen `div.container`, da es keine farblichen Abschnitte gibt 
- erster Abschnitt `section.col.content-intro` über ganze Breite 
- zweiter Abschitt ist zweispaltig 
    - `div.row` mit größerem Gutter `.gx-5` 
    - alle H2 als `.visually-hidden` 
    - Beitragsliste `section.col-md-8.beitragsliste` 
    - Linklisten als `aside.col-md-4.linklisten` 
    - Gestaltung der Artikel und Linklisten mit Bootstrap-Utilities 
- Navigationslinks aktivieren (auch auf der Startseite) 

--- 

## Seite Über uns komplett 
Template plus Content-Abschnitte für die Seite Über uns 
- `.content-intro` mit nach rechts gefloatetem Bild 
- `.team` mit Karten 
    - farbiger Header mit `card-header bg-primary` 
    - Inhalt in `card-body` 

---

## Seite Kontakt komplett 
Kontaktdaten und Kontaktformular 
- mobil untereinander 
- ab `sm` 
    - kontaktformular links 
    - kontaktdaten rechts 





--- eof --- 
