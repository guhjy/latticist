This project has moved to github: https://github.com/floybix/latticist

**latticist** is an **[R](http://www.R-project.org/)** package, providing a graphical user interface for exploratory visualisation. It is primarily an interface to the **[lattice](http://cran.r-project.org/package=lattice)** graphics system, but also produces displays from the **[vcd](http://cran.r-project.org/package=vcd)** package for categorical data. Given a multivariate dataset (either a data frame or a table), latticist attempts to produce useful displays based on the properties of the data. The displays can be customised by editing the calls used to generate them.

The latticist package is maintained by Felix Andrews `<felix@nfrac.org>`

### Examples ###
  * Screenshots of the GUI in its three flavours:
    * [gWidgets tcl/tk-based GUI](http://code.google.com/p/latticist/wiki/GuiTcltk)
    * [gWidgets RGtk2-based GUI](http://code.google.com/p/latticist/wiki/GuiRGtk2)
    * [playwith-based GUI](http://code.google.com/p/latticist/wiki/GuiPlaywith)
  * A [sequence of screenshots](http://code.google.com/p/latticist/wiki/DemoFrogs) with the playwith-based GUI.
  * Demonstrations of Latticist (outputs):
    * [Latticist CO2 demo (200k PDF)](http://latticist.googlecode.com/svn/trunk/inst/doc/latticistCO2.pdf)
    * [Latticist Frogs demo (700k PDF)](http://latticist.googlecode.com/svn/trunk/inst/doc/latticistFrogs.pdf)
    * [Latticist Aids2 demo (700k PDF)](http://latticist.googlecode.com/svn/trunk/inst/doc/latticistAids2.pdf)
    * [Latticist Employment demo (200k PDF)](http://latticist.googlecode.com/svn/trunk/inst/doc/latticistEmployment.pdf)

### Installation ###
  1. `install.packages("latticist")`
  1. Choose your Graphical User Interface. At least one of:
    * `install.packages("gWidgetstcltk")` (no external dependencies)
    * ~~`install.packages("gWidgetsrJava")`  (requires Java)~~
    * `install.packages("gWidgetsRGtk2")`  (requires GTK+)
    * `install.packages("playwith")`  (requires GTK+)
  1. `library("latticist")`

Type `latticist(myData)` to explore a data frame or table.

Type `help("latticist")` for details and examples.

### Other ###

[NEWS (from the development version)](http://code.google.com/p/latticist/source/browse/trunk/inst/NEWS)

See [this page](http://playwith.googlecode.com/) for information about installing GTK+ and the **playwith** package.