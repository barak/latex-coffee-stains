coffee
======

Coffee stains package for latex

## Usage

To use the package, simply place the `coffee.sty` file in the
directory with all of your other `.tex` files *or*
install it properly (consult your distribution's manual).  Then
include the following line in the header of your document:
```
\usepackage{coffee}
```

Since version 5, there is a convenient command:
```
\cofeSplash{}
```
to place a random splash with random parameters on the current
page. There is now also a package option to put coffee on every page like
```
\usepackage[onEveryPage]{coffee}
```

Since version 6, there is a convenient command:
```
\cofeBleed{alpha}{scale}{angle}{xoff}{yoff}{bleed}{variety}
```
to place a `variety` type splash with random parameters on the
current page. There is now also a package option to put a bleeding
coffee throughout the pages like
```
\usepackage[bleed]{coffee}
```

For more fine grained control, use the original commands:

To place a coffee stain on a page, put one of the following commands
in the source code of the relevant page:

```
\cofeAm{alpha}{scale}{angle}{xoff}{yoff}
\cofeBm{alpha}{scale}{angle}{xoff}{yoff}
\cofeCm{alpha}{scale}{angle}{xoff}{yoff}
\cofeDm{alpha}{scale}{angle}{xoff}{yoff}
```
where `alpha` is
the transparency factor $\in [0,1]$. The scale factor is `scale`,
and the standard is `scale=1`.  The angle is in degrees $\in
[0,360]$.  The position relative to the centre of the page is given by
x and y offsets `xoff` and `yoff`.



## Genesis

The latex-coffee package.

by Hanno Rein, Cambridge University

http://hanno-rein.de   hanno@hanno-rein.de


#### November, 2010

Updated to TikZ (for compatibility with pdflatex)

by Evan Sultanik, Johns Hopkins University APL

http://www.sultanik.com/ evan@sultanik.com


Inspired by several arXiv papers (see eg. 0812.3367v2)


#### March, 2011

Adding more options and  compatible with pdflatex

by Luis Randez, IUMA, University of Zaragoza

http://pcmap.unizar.es/~pilar/  randez@unizar.es


#### May, 2012

Added placement parameters

by Adrian Robson

http://nepsweb.co.uk/homeapr/


#### December, 2014

Added random \cofeSplash{} (requires ifthen) and onEveryPage package option

added to github

by Sebastian Schmittner

http://www.thp.uni-koeln.de/~ses/


#### November, 2018

Added random \cofeBleed{} (requires ifthen) and bleed package option

added to github

by Anthony Mirand

https://anthonymirand.github.io/


## License

MIT License, see LICENSE.
