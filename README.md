
# Kicad tools for Wemos D1 mini

## Updated for KiCad 8.x

All legacy files have been converted to the corresponding current KiCad 8.x 
file formats, unnecessary files have been removed. The original pin header 
symbols `CONN_01X08` have been mapped to the symbol `Connector_Generic:Conn_01x08`
included with KiCad.

## D1 Shield template
Use this template to create a new project with a D1 shield schematic and
PCB as basis.

* dowload the template directory
 `git clone ...`
* copy (or link) it to your user template directory
 * on Linux : `~/kicad/template/`
 * on Windows : `C:\Users\<USERNAME>\Documents\KiCad\8.0\template\`
 * on MacOS/OSX : `/Users/<USERNAME>/Documents/template`
* rename it as you like, e.g.: `D1_mini_Shield`

Within KiCad, create a new project from template. Select _File > New Project from Template..._

<img src="work/img/screenshot1.jpg" width=400>

The board looks like that:

<img src="template/meta/brd.png" width=400>

## D1 as component
You can also use the D1 mini as a module of a bigger KiCad PCB project.

### Symbol for KiCad
`library/wemos_mini.kicad_sym` can be used as a symbol / component in your design.

<img src="work/img/screenshot2.jpg" width=200>

To add it to KiCad:
* Go to _Preferences > Manage Symbol Libraries..._
* Choose if you want this symbol to be available globally for all your projects or only for the current project by selecting the corresponding tab
* Click the folder icon below the list (_Add existing library to table_)
* navigate to the `library/wemos_mini.kicad_sym` file
* click _Open_
* the symbol is then added to KiCad

### Footprint for KiCad

`library/wemos_d1_mini.pretty` contains a footprint of the D1 module for your PCB.

<img src="work/img/screenshot3.jpg" width=200>

To add it to KiCad:
* Go to _Preferences > Manage Footprint Libraries..._
* Choose if you want this symbol to be available globally for all your projects or only for the current project by selecting the corresponding tab
* Click the folder icon below the list (_Add existing_)
* navigate **into** the `library/wemos_d1_mini.pretty`
* click _Select Folder_
* the footprint is then added to KiCad