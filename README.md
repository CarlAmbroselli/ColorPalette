# ColorPalette

This repository contains the source code of the CRAN Package [ColorPalette](http://cran.r-project.org/web/packages/ColorPalette/). 

# Installation
It can be installed from CRAN or directly from GitHub:

~~~ R
install.packages("devtools")
library("devtools")
devtools::install_github("carlambroselli/ColorPalette")
~~~

# API


### hsv2rgb(h,s,v) 
This function converts the values of a color from hsv color space to rgb.
~~~
@param h Hue of the color
@param s Saturation of the color
@param v Value of the color
@keywords hsv rgb
@export
@examples
hsv2rgb(150,0.2,0.6)
~~~

### complement(hex, typeVal="")
This function returns the complement color of a rgb color
~~~
@param hex The base color specified as hex
@param typeVal Can be specified as split or double. Default is empty.
@keywords complement
@export
@examples
complement("#121314")
~~~

### triadic(hex)
This function returns triadic colors to a given hex color
~~~
@param hex The base color specified as hex
@keywords triadic
@export
@examples
triadic("#121314")
~~~

### tetradic(hex)
This function returns tetradic colors to a given hex color
~~~
@param hex The base color specified as hex
@keywords tetradic
@export
@examples
tetradic("#121314")
~~~

### pentadic(hex)
This function returns pentadic colors to a given hex color
~~~
@param hex The base color specified as hex
@keywords pentadic
@export
@examples
pentadic("#121314")
~~~

### generateMonochromaticColors(baseColor, count)
This function generates a specified number of monochromatic colors for a given base color
~~~
@param baseColor The base color specified as hex
@param count Number of colors the palette should contain
@keywords monochromatic color
@export
@examples
generateMonochromaticColors("#121314", 5)
~~~

### complementColors(baseColor, count)
This function generates a color plate with the complement color
~~~
@param baseColor The base color specified as hex
@param count Number of colors the palette should contain
@keywords complement color
@export
@examples
complementColors("#121314", 5)
~~~

### triadicColors(baseColor, count)
This function generates a specified number of triadic colors for a given base color
~~~
@param baseColor The base color specified as hex
@param count Number of colors the palette should contain
@keywords triadic color
@export
@examples
triadicColors("#121314", 5)
~~~

### tetradicColors(baseColor, count)
This function generates a specified number of tetradic colors for a given base color
~~~
@param baseColor The base color specified as hex
@param count Number of colors the palette should contain
@keywords tetradic color
@export
@examples
tetradicColors("#121314", 5)
~~~
