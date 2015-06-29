Rachel Andrew - "The New CSS Layout"
====================================

I’m very excited about the possibilities that await us by way of proposed layout modules for CSS. While some of these 
modules are at an early stage, I believe it is important that designers and developers start to look at, play with and 
discuss these proposals. If we don’t then we can’t complain when the final specifications don’t meet our needs.

This talk is based on the work I did for my CSS Layout Modules Pocket Guide and covers Multi-column Layout, Flexbox, 
Grid, Regions, Exclusions and Shapes.

Sources
-------

 * Talk: <http://www.slideshare.net/rachelandrew/the-new-css-layout-dutch-php-conference>
 * Twitter: <https://twitter.com/rachelandrew>
 * Github: <https://github.com/rachelandrew>

Notes
-----

 * Multicolumn
 
   * Spalten-Layout
   * Gute Unterstützung über alle Browser <http://caniuse.com/#feat=multicolumn>
   * "column-with: 200px" werden nicht genau 200px sein
   * "column-span: all|none" nur alles oder nichts
   * Einsatzmöglichkeiten:

     * Zeitungslayout
     * UI für das Anordnen der Checkbox horizontal

 * Flexbox

   * Gute Unterstützung über alle Browser <http://caniuse.com/#feat=flexbox>
   * Anordnung von Elementen horizontal
   * Alle Element bekommen die gleiche Höhe
   * Änderung der Reihnfolge vom Elementen
   * Kaum gute Beispiele im Internet, da sich die Spezifikation geändert hat
   * Umgang mit Reponsive Images nur mit "min-width: 1px" möglich sonst brechen die Bilder aus
   * Einsatzmöglichkeiten:

     * Horizontale Navigation

 * Shapes
   * Textfluss um Bilder

     * Circle, Elipse, Polygon, Alpha-Channel

   * Schlechte Unterstützung, nur Blink <http://caniuse.com/#feat=css-shapes>
   
   
 * Grid

   * Grid Layout mit der Möglichkeit Elemente zu Positionieren und die Reihenfolge zu ändern
   * Schlechte Unterstützung, nur IE/Edge <http://caniuse.com/#feat=css-grid>

 * Exclusions

   * Änderung des Textfluss mittles absolute positionierter Elemente
   * Schlechte Unterstützung, nur IE/Edge <http://caniuse.com/#feat=css-exclusions>

 * Regions

   * Testfluss Kontrolle über mehrere leere Container
   * Schlechte Unterstützung, Webkit | IE/Edge <http://caniuse.com/#feat=css-regions> 
