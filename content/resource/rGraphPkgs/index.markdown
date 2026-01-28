---
title: "List of R packages to create and edit plots"
wikitheme: R
date: 2015-12-04
update: 2023-02-10
categories: [about R]
tags: [plot, R, wiki]
draft: false
tweet: "List of R packages to create and edit plots"
output:
  rmarkdown::html_page:
    toc: true
    fig_width: 3
    dev: svglite
---

Note that the list of packages below would be updated as soon as we find a new
package. If you know a package that should be in the list, please feel mention
it in the comment section below.

<br/>

## Why use R to produce graphics?

S, R's ancestor, was first designed to be an interactive interface for calling routines from the SCS (Statistical Computing Subroutines) FORTRAN library. It expanded to be a complete programming language dedicated to data manipulation, statistical analysis and data visualization (see [A brief History of S](http://www.lcg.unam.mx/~lcollado/R/resources/history_of_S.pdf)). Today's graphical system of R is directly derived from the one of S. When R is installed, you get from it two base packages, ['graphics'](https://stat.ethz.ch/R-manual/R-devel/library/graphics/html/00Index.html) and ['grid'](https://stat.ethz.ch/R-manual/R-devel/library/grid/html/00Index.html), which produce graphics that are exported with the [grDevices](https://stat.ethz.ch/R-manual/R-devel/library/grDevices/html/00Index.html) package. These packages are very complete and flexible. They allow users to efficiently create graphics that scientists use in their day to day operations, *i.e.* scatterplots, box plots, histograms, etc. We consider that the 'graphics' package is somewhat more user-friendly than the trickier 'grid' package which offers better facilities to develop new graphical functions (e.g. grid' has been employed to build [ggplot2](https://cran.r-project.org/web/packages/ggplot2)). Recently, the [gridGraphics](https://journal.r-project.org/archive/2015-1/murrell.pdf) package has been developed to bridge the gap between 'grid' and 'graphics' packages.

That being said, the advantages are numerous and more can be built in. For instance:


1. You get all the advantages linked with using R, *i.e.* it is free, lot of documentation exists, a very large community of users, there are many packages, it is easy to learn.

2. Any kind of graphics a scientist needs has already been implemented by many contributors (see the packages review below). If you find there is room for improvement or that we are mistaken, all information is available to further develop missing plotting functions or correct existing ones.

3. Almost everything is possible. All graphics are fully customizable. Some time is required to learn the works, but it's worth it.

4. Although there may be many good reasons to use software to post-treat graphics R produces in WYSIWYG softwares, we contend that once you master R, you will never do so. When a graphics is done, it is associated with only a few lines of code. Changing solely the lines of code is a much more efficient way more efficient to solve any problem than reproducing and post-treating the graphics. As scientists, it is a victory to only modify a few lines of code when reviewers quibble about a figure.

5. Once a graphics is created, we can export it in many formats: `.eps`, `.jpeg`, `.pdf`, `.bmp`, `.svg` with appropriate resolution and size. There is 100% guarantee that you will meet a journal's requirements for figures publication.




## Documentation

We will make the content below 'evolving' by collecting and indexing as many sources of documentation as possible. Please comment in the Disqus section below to suggest and/or provide your own sources:


- **Comprehensive R Archive Network** ([CRAN](https://cran.r-project.org))
    - [Manuals](https://cran.r-project.org/manuals.html)
    - [Contributed manuals and cheat sheets](https://cran.r-project.org/other-docs.html)

- **Journals**
    - [R journal](https://journal.r-project.org)
    - [Journal of Statistical Software](http://www.jstatsoft.org/index)

- **Books**:
    - [Fundamentals of Data Visualization](https://clauswilke.com/dataviz/)
    - [Data Visualizatio](https://socviz.co/)
    - [Rgraphics, Second  Edition](https://www.stat.auckland.ac.nz/~paul/RG2e/index.html)
    - [R Graphics Cookbook](http://www.cookbook-r.com/Graphs/)

- **Blogs**:
    - [R-bloggers](http://www.r-bloggers.com)
    - [inside-R](http://www.inside-r.org)
    - [Quick-R](http://www.statmethods.net/about/learningcurve.html)
    - [Revolutions](http://blog.revolutionanalytics.com/about.html)
    - [The R Graph Gallery](https://r-graph-gallery.com/)

- **ggplot2**:
    - [ggplot2 (book)](https://ggplot2-book.org/)
    - [liste of extensions](https://exts.ggplot2.tidyverse.org/)



## List of packages

<!-- Find package [here](http://rpackages.ianhowson.com) A comprehensive index of R packages and documentation from CRAN, Bioconductor, GitHub and R-Forge. (https://cran.r-project.org/web/packages/available_packages_by_name.html) -->
Many packages for graphics are indexed in a dedicated [task view maintained by Nicholas Lewin-Koh](https://cran.r-project.org/web/views/Graphics.html) and many ggplot2 extensions are listed on [ggplot2 extensions](https://www.ggplot2-exts.org/). We have indexed many of them and refer to more below. For each package, we provide:

  - the name of the package with a link that goes to the [CRAN](https://cran.r-project.org) repository where the manual and optional vignettes can be found,
  - a text summarizing the package content (an adequate part of the description found online),

when available, we also provide :

  - <a href=""><i class="fab fa-github"></i></a>: a link that goes to the [Github](https://github.com) repository,
  - <a href=""><i class="fab fa-bitbucket"></i></a>: a link that goes to the associated [Bitbucket](https://bitbucket.org) repository,
  - <a href=""><i class="ai ai-doi"></i></a>: a link that goes to the [DOI](http://www.doi.org) link,
  - <a href=""><i class="fas fa-link"></i></a>: a link that goes to a dedicated website, a html vignette that describes well the package or a relevant publication,
  - <a href=""><i class="fas fa-file-pdf"></i></a>: a link that goes to an relevant pdf file (an R journal article for instance).



## Main packages
1. **plotrix** lots of plots, various labeling, axis and color scaling functions. [CRAN](https://cran.r-project.org/web/packages/plotrix) <a href='https://r-forge.r-project.org/projects/plotrix'><i class='fas fa-link'></i></a> <a href='https://www.r-project.org/doc/Rnews/Rnews_2006-4.pdf'><i class='fas fa-file-pdf'></i></a>
2. **gplots** various R Programming Tools for Plotting Data. [CRAN](https://cran.r-project.org/web/packages/gplots)
3. **lattice** R implementation of Trellis Graphics. [CRAN](https://cran.r-project.org/web/packages/lattice) <a href='http://r-forge.r-project.org/projects/lattice/'><i class='fas fa-link'></i></a>
4. **ggplot2** an implementation of the grammar of graphics in R (see below for extensions). [CRAN](https://cran.r-project.org/web/packages/ggplot2) <a href='https://github.com/hadley/ggplot2'><i class='fab fa-github'></i></a> <a href='http://ggplot2.org'><i class='fas fa-link'></i></a>
<br/> 

## Colors
1. **colorspace** a package for color space manipulation. [CRAN](https://cran.r-project.org/web/packages/colorspace)
2. **colourlovers** Provides access to the COLOURlovers API, which offers color inspiration and color palettes. [CRAN](https://cran.r-project.org/web/packages/colourlovers) <a href='https://github.com/leeper/colourlovers'><i class='fab fa-github'></i></a>
3. **dichromat** collapses red-green or green-blue distinctions to simulate the effects of different types of color-blindness. [CRAN](https://cran.r-project.org/web/packages/dichromat)
4. **munsell** provides easy access to, and manipulation of, the Munsell colours. [CRAN](https://cran.r-project.org/web/packages/munsell)
5. **RColorBrewer** provides color schemes for maps (and other graphics) designed by Cynthia Brewer. [CRAN](https://cran.r-project.org/web/packages/RColorBrewer)
6. **RImagePalette**  extracts the dominant colors from an image, and turns them into a scale for use in plots or for fun! [CRAN](https://cran.r-project.org/web/packages/RImagePalette)
7. **scales** scale functions for visualization. [CRAN](https://cran.r-project.org/web/packages/scales) <a href='https://github.com/hadley/scales'><i class='fab fa-github'></i></a>
8. **viridis** port of the new 'matplotlib' color maps to 'R' [CRAN](https://cran.r-project.org/web/packages/viridis) <a href='https://github.com/sjmgarnier/viridis'><i class='fab fa-github'></i></a> <a href='https://cran.r-project.org/web/packages/viridis/vignettes/intro-to-viridis.html'><i class='fas fa-link'></i></a>
9. **viridisLite** viridis Lite version [CRAN](https://cran.r-project.org/web/packages/viridisLite) <a href='https://github.com/sjmgarnier/viridisLite'><i class='fab fa-github'></i></a>
10. **wesanderson** palettes generated mostly from Wes Anderson movies. [CRAN](https://cran.r-project.org/web/packages/wesanderson) <a href='https://github.com/karthik/wesanderson'><i class='fab fa-github'></i></a>
<br/> 

## Fonts
1. **extrafont** tools to using fonts other than the standard PostScript fonts. [CRAN](https://cran.r-project.org/web/packages/extrafont) <a href='https://github.com/https://github.com/wch/extrafont'><i class='fab fa-github'></i></a>
2. **showtext** eases the use of fonts in R graphs. [CRAN](https://cran.r-project.org/web/packages/showtext) <a href='https://github.com/yixuan/showtext'><i class='fab fa-github'></i></a> <a href='https://journal.r-project.org/archive/2015-1/qiu.pdf'><i class='fas fa-file-pdf'></i></a>
3. **emojifont** an implementation of using emoji font in both base and 'ggplot2' graphics. [CRAN](https://cran.r-project.org/web/packages/emojifont) <a href='https://github.com/GuangchuangYu/emojifont'><i class='fab fa-github'></i></a> <a href='https://cran.r-project.org/web/packages/emojifont/vignettes/emojifont.html'><i class='fas fa-link'></i></a>
4. **hexSticker** an implementation of using emoji font in both base and 'ggplot2' graphics. [CRAN](https://cran.r-project.org/web/packages/hexSticker) <a href='https://github.com/GuangchuangYu/hexSticker'><i class='fab fa-github'></i></a>
<br/> 

## Extra plot functions
1. **ade4** multivariate data analysis of ecological data and graphical display associated. [CRAN](https://cran.r-project.org/web/packages/ade4) <a href='https://github.com//sdray/ade4'><i class='fab fa-github'></i></a> <a href='http://pbil.univ-lyon1.fr/ADE-4/'><i class='fas fa-link'></i></a>
2. **adegraphics** graphical functionalities for the representation of multivariate data (complete re-implementation of the functions available in the 'ade4' package). [CRAN](https://cran.r-project.org/web/packages/adegraphics) <a href='https://github.com/sdray/adegraphics'><i class='fab fa-github'></i></a> <a href='https://cran.r-project.org/web/packages/adegraphics/vignettes/adegraphics.html'><i class='fas fa-link'></i></a> <a href='https://journal.r-project.org/archive/2017/RJ-2017-042/RJ-2017-042.pdf'><i class='fas fa-file-pdf'></i></a>
3. **aplpack** a set of functions for drawing some special plots [CRAN](https://cran.r-project.org/web/packages/aplpack)
4. **beanplot** visualization via Beanplots. [CRAN](https://cran.r-project.org/web/packages/beanplot)
5. **circlize** provides an implementation of circular layout generation in R as well as an enhancement of available software. [CRAN](https://cran.r-project.org/web/packages/circlize) <a href='https://github.com/jokergoo/circlize'><i class='fab fa-github'></i></a> <a href='http://zuguang.de/circlize/'><i class='fas fa-link'></i></a> <a href='https://cran.r-project.org/web/packages/circlize/vignettes/circlize.pdf'><i class='fas fa-file-pdf'></i></a>
6. **corrgram** calculates correlation of variables and displays the results graphically. [CRAN](https://cran.r-project.org/web/packages/corrgram) <a href='https://github.com/kwstat/corrgram'><i class='fab fa-github'></i></a> <a href='https://cran.r-project.org/web/packages/corrgram/vignettes/corrgram_examples.pdf'><i class='fas fa-link'></i></a>
7. **corrplot** graphical display of a correlation matrix, confidence interval. [CRAN](https://cran.r-project.org/web/packages/corrplot) <a href='https://github.com//taiyun/corrplot'><i class='fab fa-github'></i></a> <a href='https://cran.r-project.org/web/packages/corrplot/vignettes/corrplot-intro.html'><i class='fas fa-link'></i></a>
8. **dendextend** offers a set of functions for extending dendrogram objects in R, letting you visualize and compare trees of hierarchical clusterings. [CRAN](https://cran.r-project.org/web/packages/dendextend) <a href='https://github.com/talgalili/dendextend'><i class='fab fa-github'></i></a> <a href='https://doi.org/10.1093/bioinformatics/btv428'><i class='ai ai-doi'></i></a>
9. **denstrip** density strips and other methods for compactly illustrating distributions. [CRAN](https://cran.r-project.org/web/packages/denstrip)
10. **genoPlotR** plot publication-grade gene and genome maps. [CRAN](https://cran.r-project.org/web/packages/genoPlotR) <a href='http://genoplotr.r-forge.r-project.org'><i class='fas fa-link'></i></a>
11. **heatmap3** provides improved heatmaps. [CRAN](https://cran.r-project.org/web/packages/heatmap3) <a href='https://cran.r-project.org/web/packages/heatmap3/vignettes/vignette.pdf'><i class='fas fa-link'></i></a>
12. **hexbin** binning and plotting functions for hexagonal bins. [CRAN](https://cran.r-project.org/web/packages/hexbin) <a href='https://github.com/edzer/hexbin'><i class='fab fa-github'></i></a> <a href='https://cran.r-project.org/web/packages/hexbin/vignettes/hexagon_binning.pdf'><i class='fas fa-file-pdf'></i></a>
13. **kohonen** Functions to train supervised and self-organising maps (SOMs). [CRAN](https://cran.r-project.org/web/packages/kohonen)
14. **pheatmap** implementation of heatmaps that offers more control over dimensions and appearance [CRAN](https://cran.r-project.org/web/packages/pheatmap)
15. **riverplot** implements Sankey or Ribbon plots. [CRAN](https://cran.r-project.org/web/packages/riverplot)
16. **sinaplot** enhanced chart for simple and truthful representation of single observations over multiple classes. [CRAN](https://cran.r-project.org/web/packages/sinaplot) <a href='https://cran.r-project.org/web/packages/sinaplot/vignettes/SinaPlot.html'><i class='fas fa-link'></i></a>
17. **sjPlot** a collection of plotting and table output functions for data visualization dediacted to statistics in social science. [CRAN](https://cran.r-project.org/web/packages/sjPlot) <a href='https://github.com/sjPlot/devel'><i class='fab fa-github'></i></a> <a href='http://strengejacke.de/sjPlot/'><i class='fas fa-link'></i></a>
18. **vcd** visualization techniques, data sets, summary and inference procedures aimed particularly at categoricaldata. [CRAN](https://cran.r-project.org/web/packages/vcd) <a href='https://doi.org/10.18637/jss.v017.i03'><i class='ai ai-doi'></i></a>
19. **Violin plot** creates Violin plots. [CRAN](https://cran.r-project.org/web/packages/Violin plot)
20. **visreg** visualization of regression models. [CRAN](https://cran.r-project.org/web/packages/visreg) <a href='https://github.com/pbreheny/visreg'><i class='fab fa-github'></i></a> <a href='http://myweb.uiowa.edu/pbreheny/publications/visreg.pdf'><i class='fas fa-file-pdf'></i></a>
<br/> 

## Clusters and trees
1. **ape** analyses of Phylogenetics and Evolution, to draw a tree see `plot.phylo()` and `plot.multiPhylo()` functions. [CRAN](https://cran.r-project.org/web/packages/ape)
2. **gclust** orders panels in scatterplot matrices and parallel coordinate displays by some merit index. [CRAN](https://cran.r-project.org/web/packages/gclust)
3. **biclust** algorithms to find biclusters in two-dimensional data, visualisation solutions are included. [CRAN](https://cran.r-project.org/web/packages/biclust)
4. **VisuClust** visualisation of Clusters in Multivariate Data. [CRAN](https://cran.r-project.org/web/packages/VisuClust)
<br/> 

## Plots in 3D
1. **plot3D** functions for viewing 2-D and 3-D data, including perspective plots, slice plots, surface plots, scatter plots, etc. [CRAN](https://cran.r-project.org/web/packages/plot3D)
2. **misc3d** a collection of miscellaneous 3d plots, including isosurfaces. [CRAN](https://cran.r-project.org/web/packages/misc3d)
3. **rgl** implements 3D visualization using OpenGL. [CRAN](https://cran.r-project.org/web/packages/rgl) <a href='https://cran.r-project.org/web/packages/rgl/vignettes/rgl.html'><i class='fas fa-link'></i></a>
4. **scatterplot3d** plots a three dimensional (3D) point cloud. [CRAN](https://cran.r-project.org/web/packages/scatterplot3d)
<br/> 

## Graph diagrams, flowcharts and networks
1. **DiagrammeR** creates network graph diagrams. [CRAN](https://cran.r-project.org/web/packages/DiagrammeR) <a href='https://github.com/rich-iannone/DiagrammeR'><i class='fab fa-github'></i></a> <a href='http://rich-iannone.github.io/DiagrammeR/'><i class='fas fa-link'></i></a>
2. **visNetwork** network visualization, using 'vis.js' javascript library. [CRAN](https://cran.r-project.org/web/packages/visNetwork) <a href='https://github.com/atastorm-open/visNetwork'><i class='fab fa-github'></i></a> <a href='https://cran.r-project.org/web/packages/visNetwork/vignettes/Introduction-to-visNetwork.html'><i class='fas fa-link'></i></a>
3. **diagram** visualising simple graphs, flowcharts, and webs. [CRAN](https://cran.r-project.org/web/packages/diagram)
4. **igraph** network analysis and visualization. [CRAN](https://cran.r-project.org/web/packages/igraph)
5. **qgraph** visualizing data as networks as well as provides an interface for visualizing weighted graphical models. [CRAN](https://cran.r-project.org/web/packages/qgraph) <a href='http://sachaepskamp.com/qgraph'><i class='fas fa-link'></i></a>
6. **shape** functions for plotting graphical shapes, colors. [CRAN](https://cran.r-project.org/web/packages/shape)
7. **VennDiagram** a set of functions to generate high-resolution Venn and Euler plots. [CRAN](https://cran.r-project.org/web/packages/VennDiagram)
<br/> 

## Maps
1. **cartography** create and integrate maps in your R workflow. [CRAN](https://cran.r-project.org/web/packages/cartography) <a href='https://github.com/Groupe-ElementR/cartography'><i class='fab fa-github'></i></a>
2. **leafletR** creates interactive web-maps based on the Leaflet JavaScript library. [CRAN](https://cran.r-project.org/web/packages/leafletR) <a href='https://github.com/chgrl/leafletR'><i class='fab fa-github'></i></a>
3. **leaflet** creates interactive web maps with the JavaScript 'Leaflet' library [CRAN](https://cran.r-project.org/web/packages/leaflet) <a href='https://github.com/rstudio/leaflet'><i class='fab fa-github'></i></a> <a href='http://rstudio.github.io/leaflet/'><i class='fas fa-link'></i></a>
4. **osmar** a package to use Open Street Map in R. [CRAN](https://cran.r-project.org/web/packages/osmar) <a href='hhttp://osmar.r-forge.r-project.org'><i class='fas fa-link'></i></a> <a href='https://journal.r-project.org/archive/2013-1/eugster-schlesinger.pdf'><i class='fas fa-file-pdf'></i></a>
5. **plotGoogleMaps** accesses high resolution raster maps using the OpenStreetMap protocol. [CRAN](https://cran.r-project.org/web/packages/plotGoogleMaps) <a href='http://r-forge.r-project.org/projects/plotgooglemaps/'><i class='fas fa-link'></i></a>
6. **maps** draws geographical maps. [CRAN](https://cran.r-project.org/web/packages/maps) <a href='http://r-forge.r-project.org/projects/maptools/'><i class='fas fa-link'></i></a>
7. **maptools** a set of tools for manipulating and reading geographic data, in particular ESRI shapefiles. [CRAN](https://cran.r-project.org/web/packages/maptools) <a href='http://r-forge.r-project.org/projects/maptools/'><i class='fas fa-link'></i></a>
8. **mapview** interactive viewing of spatial data in R. [CRAN](https://cran.r-project.org/web/packages/mapview) <a href='https://github.com/r-spatial/mapview'><i class='fab fa-github'></i></a> <a href='https://r-spatial.github.io/mapview/'><i class='fas fa-link'></i></a>
9. **micromap** a package for linked micromaps. [CRAN](https://cran.r-project.org/web/packages/micromap) <a href='https://doi.org/10.18637/jss.v063.i02'><i class='ai ai-doi'></i></a>
10. **raster** reading, writing, manipulating, analyzing and modeling of gridded spatial data. [CRAN](https://cran.r-project.org/web/packages/raster) <a href='https://cran.r-project.org/web/packages/raster/vignettes/Raster.pdf'><i class='fas fa-file-pdf'></i></a>
11. **rgdal** reads shapefiles and rasters using Frank Warmerdam's Geospatial Data Abstraction Library. [CRAN](https://cran.r-project.org/web/packages/rgdal) <a href='https://r-forge.r-project.org/projects/rgdal/'><i class='fas fa-link'></i></a>
<br/> 

## Interactive graphics
1. **iplot** interactive graphics for R. [CRAN](https://cran.r-project.org/web/packages/iplot) <a href='http://www.iPlots.org/'><i class='fas fa-link'></i></a>
2. **manipulate** interactive plotting functions for use within RStudio. [CRAN](https://cran.r-project.org/web/packages/manipulate) <a href='https://github.com/rstudio/manipulate'><i class='fab fa-github'></i></a> <a href='https://support.rstudio.com/hc/en-us/articles/200551906-Interactive-Plotting-with-Manipulate'><i class='fas fa-link'></i></a>
3. **playwith** a GUI for interactive plots using GTK+ [CRAN](https://cran.r-project.org/web/packages/playwith) <a href='http://playwith.googlecode.com/'><i class='fas fa-link'></i></a>
4. **rpanel** simple interactive controls for R using the tcltk library. [CRAN](https://cran.r-project.org/web/packages/rpanel) <a href='http://www.stats.gla.ac.uk/~adrian/rpanel/'><i class='fas fa-link'></i></a> <a href='https://doi.org/10.18637/jss.v017.i09'><i class='ai ai-doi'></i></a> <a href='https://cran.r-project.org/doc/Rnews/Rnews_2006-4.pdf'><i class='fas fa-file-pdf'></i></a>
<br/> 

## Image importation and image processing
1. **bmp** reads Windows BMP format images [CRAN](https://cran.r-project.org/web/packages/bmp)
2. **grImport** a set of functions for converting, importing, and drawing PostScript pictures in R plots. [CRAN](https://cran.r-project.org/web/packages/grImport) <a href='https://doi.org/10.18637/jss.v030.i04'><i class='ai ai-doi'></i></a> <a href='https://cran.r-project.org/web/packages/grImport/vignettes/import.pdf'><i class='fas fa-file-pdf'></i></a>
3. **imager** Image Processing Library Based on 'CImg [CRAN](https://cran.r-project.org/web/packages/imager) <a href='https://github.com/dahtah/imager'><i class='fab fa-github'></i></a> <a href='http://dahtah.github.io/imager/'><i class='fas fa-link'></i></a>
4. **jpeg** reads bitmap images stored in the JPEG format. [CRAN](https://cran.r-project.org/web/packages/jpeg) <a href='http://www.rforge.net/jpeg/'><i class='fas fa-link'></i></a>
5. **pixmap** functions for import, export, plotting and other manipulations of bitmapped images. [CRAN](https://cran.r-project.org/web/packages/pixmap)
6. **png** Reads bitmap images stored in the PNG format. [CRAN](https://cran.r-project.org/web/packages/png) <a href='http://www.rforge.net/png/'><i class='fas fa-link'></i></a>
<br/> 

## ggplot2 and extensions
1. **ggplot2** an implementation of the grammar of graphics in R. [CRAN](https://cran.r-project.org/web/packages/ggplot2) <a href='https://github.com/hadley/ggplot2'><i class='fab fa-github'></i></a> <a href='http://ggplot2.org'><i class='fas fa-link'></i></a>
2. **cowplot** provide a publication-ready theme for ggplot2 [CRAN](https://cran.r-project.org/web/packages/cowplot) <a href='https://github.com/wilkelab/cowplot'><i class='fab fa-github'></i></a> <a href='https://cran.r-project.org/web/packages/cowplot/vignettes/introduction.html'><i class='fas fa-link'></i></a>
3. **ggthemes** some extra themes, geoms, and scales for 'ggplot2' [CRAN](https://cran.r-project.org/web/packages/ggthemes) <a href='https://github.com//jrnold/ggthemes'><i class='fab fa-github'></i></a> <a href='https://cran.r-project.org/web/packages/ggthemes/vignettes/ggthemes.html'><i class='fas fa-link'></i></a>
4. **GGally** extension to ggplot2. [CRAN](https://cran.r-project.org/web/packages/GGally) <a href='http://ggobi.github.io/ggally/'><i class='fas fa-link'></i></a>
5. **ggbeeswarm** beeswarm-style plots with ggplot2. [CRAN](https://cran.r-project.org/web/packages/ggbeeswarm) <a href='https://github.com/eclarke/ggbeeswarm'><i class='fab fa-github'></i></a>
6. **ggridges** visualize changes in distributions over time or space. [CRAN](https://cran.r-project.org/web/packages/ggridges) <a href='https://github.com/clauswilke/ggridges'><i class='fab fa-github'></i></a> <a href='https://cran.r-project.org/web/packages/ggridges/vignettes/gallery.html'><i class='fas fa-link'></i></a>
7. **ggcorrplot** visualization of a correlation matrix using ggplot2 [CRAN](https://cran.r-project.org/web/packages/ggcorrplot) <a href='https://github.com/kassambara/ggcorrplot'><i class='fab fa-github'></i></a>
8. **ggdendro** a set of tools for dendrograms and tree plots using 'ggplot2'. [CRAN](https://cran.r-project.org/web/packages/ggdendro) <a href='https://github.com/andrie/ggdendro'><i class='fab fa-github'></i></a> <a href='https://cran.r-project.org/web/packages/ggdendro/vignettes/ggdendro.html'><i class='fas fa-link'></i></a>
9. **gge** creates biplots for GGE (genotype plus genotype-by-environment) and GGB (genotype plus genotype-by-block-of-environments) models. [CRAN](https://cran.r-project.org/web/packages/gge)
10. **GGEBiplotGUI** interactive GGE Biplots in R [CRAN](https://cran.r-project.org/web/packages/GGEBiplotGUI)
11. **ggenealogy** visualization tools for genealogical data. [CRAN](https://cran.r-project.org/web/packages/ggenealogy)
12. **ggExtra** adds marginal histograms to ggplot2, and more ggplot2 enhancements. [CRAN](https://cran.r-project.org/web/packages/ggExtra) <a href='https://github.com//daattali/ggExtra'><i class='fab fa-github'></i></a> <a href='https://cran.r-project.org/web/packages/ggExtra/vignettes/overview.html'><i class='fas fa-link'></i></a>
13. **ggforce** ggforce is a package aimed at providing missing functionality to ggplot2 through the extension system introduced with ggplot2 v2.0.0. [CRAN](https://cran.r-project.org/web/packages/ggforce) <a href='https://github.com/thomasp85/ggforce'><i class='fab fa-github'></i></a>
14. **ggiraph** creates interactive 'ggplot2' graphics that are usable in the 'RStudio' viewer pane, in 'R Markdown' documents and in 'Shiny' apps. [CRAN](https://cran.r-project.org/web/packages/ggiraph) <a href='https://github.com/davidgohel/ggiraph'><i class='fab fa-github'></i></a>
15. **ggmap** a collection of functions to visualize spatial data and models on top of static maps from various online sources. [CRAN](https://cran.r-project.org/web/packages/ggmap) <a href='https://github.com/dkahle/ggmap'><i class='fab fa-github'></i></a>
16. **ggnetwork** geometries to plot network objects with 'ggplot2'. [CRAN](https://cran.r-project.org/web/packages/ggnetwork) <a href='https://github.com/briatte/ggnetwork'><i class='fab fa-github'></i></a> <a href='https://cran.r-project.org/web/packages/ggnetwork/vignettes/ggnetwork.html'><i class='fas fa-link'></i></a>
17. **ggparallel** creates hammock plots, parallel sets, and common angle plots with ggplot2. [CRAN](https://cran.r-project.org/web/packages/ggparallel) <a href='https://github.com/heike/ggparallel'><i class='fab fa-github'></i></a>
18. **ggpmisc** extensions to 'ggplot2' respecting the grammar of graphics paradigm. [CRAN](https://cran.r-project.org/web/packages/ggpmisc) <a href='https://bitbucket.org/aphalo/ggpmisc'><i class='fab fa-bitbucket'></i></a> <a href='https://cran.r-project.org/web/packages/ggpmisc/vignettes/examples.html'><i class='fas fa-link'></i></a>
19. **ggRandomForests** graphic elements for exploring Random Forests. [CRAN](https://cran.r-project.org/web/packages/ggRandomForests) <a href='https://github.com/ehrlinger/ggRandomForests'><i class='fab fa-github'></i></a>
20. **ggraptR** allows Interactive Visualization of Data Through a Web Browser GUI. [CRAN](https://cran.r-project.org/web/packages/ggraptR) <a href='https://github.com/cargomoose/raptR'><i class='fab fa-github'></i></a>
21. **ggrepel** provides text and label geoms for 'ggplot2' that help to avoid overlapping text labels. [CRAN](https://cran.r-project.org/web/packages/ggrepel) <a href='https://github.com/slowkow/ggrepel'><i class='fab fa-github'></i></a> <a href='https://cran.r-project.org/web/packages/ggrepel/vignettes/ggrepel.html'><i class='fas fa-link'></i></a>
22. **ggROC** a package for roc curve plot with ggplot2. [CRAN](https://cran.r-project.org/web/packages/ggROC)
23. **ggsci** scientific journal and Sci-Fi themed volor palettes for 'ggplot2'. [CRAN](https://cran.r-project.org/web/packages/ggsci) <a href='https://github.com/road2stat/ggsci'><i class='fab fa-github'></i></a> <a href='http://ggsci.net'><i class='fas fa-link'></i></a>
24. **ggseas** seasonal adjustment on the fly extension for ggplot2. [CRAN](https://cran.r-project.org/web/packages/ggseas) <a href='https://github.com/ellisp/ggseas'><i class='fab fa-github'></i></a>
25. **ggsn** adds north symbols and scale bars to maps created with 'ggplot2' or 'ggmap'. [CRAN](https://cran.r-project.org/web/packages/ggsn) <a href='https://github.com/oswaldosantos/ggsn'><i class='fab fa-github'></i></a> <a href='http://oswaldosantos.github.io/ggsn/'><i class='fas fa-link'></i></a>
26. **ggspectra** extensions to 'ggplot2' for Radiation Spectra [CRAN](https://cran.r-project.org/web/packages/ggspectra) <a href='https://bitbucket.org//aphalo/ggspectra'><i class='fab fa-bitbucket'></i></a> <a href='https://cran.r-project.org/web/packages/ggspectra/index.html'><i class='fas fa-link'></i></a>
27. **ggtern** an Extension to 'ggplot2', for the creation of ternary diagrams. [CRAN](https://cran.r-project.org/web/packages/ggtern) <a href='https://bitbucket.org/nicholasehamilton/ggtern'><i class='fab fa-bitbucket'></i></a> <a href='http://www.ggtern.com'><i class='fas fa-link'></i></a>
28. **ggThemeAssist** Rstudio add-in that delivers a graphical interface for editing 'ggplot2' theme elements. [CRAN](https://cran.r-project.org/web/packages/ggThemeAssist) <a href='https://github.com/calligross/ggthemeassist'><i class='fab fa-github'></i></a>
29. **ggvis** an implementation of an interactive grammar of graphics. [CRAN](https://cran.r-project.org/web/packages/ggvis) <a href='https://github.com/rstudio/ggvis'><i class='fab fa-github'></i></a> <a href='http://ggvis.rstudio.com'><i class='fas fa-link'></i></a>
30. **gg3D** a ggplot2 extension enabling 3D projections. [CRAN](https://cran.r-project.org/web/packages/gg3D) <a href='https://github.com/AckerDWM/gg3D'><i class='fab fa-github'></i></a>
31. **lemon** functions for working with legends and axis lines of 'ggplot2', facets that repeat axis lines on all panels, and some 'knitr' extensions. [CRAN](https://cran.r-project.org/web/packages/lemon) <a href='https://github.com/stefanedwards/lemon'><i class='fab fa-github'></i></a>
<br/> 

## Miscellaneous
1. **arulesViz** visualizing association rules and frequent itemsets. [CRAN](https://cran.r-project.org/web/packages/arulesViz) <a href='https://github.com/mhahsler/arules'><i class='fab fa-github'></i></a> <a href='https://doi.org/10.18637/jss.v014.i15'><i class='ai ai-doi'></i></a> <a href='https://cran.r-project.org/web/packages/arulesViz/vignettes/arulesViz.pdf'><i class='fas fa-file-pdf'></i></a>
2. **animation** a gallery of animations in statistics and utilities to create animations. [CRAN](https://cran.r-project.org/web/packages/animation) <a href='https://github.com/Yihui/animation'><i class='fab fa-github'></i></a>
3. **move** visualizing and analyzing animal track data. [CRAN](https://cran.r-project.org/web/packages/move) <a href='http://computational-ecology.com/main-move.html'><i class='fas fa-link'></i></a>
4. **personographs** visualizes treatment effects using person icons, similar to Cates (NNT) charts. [CRAN](https://cran.r-project.org/web/packages/personographs) <a href='https://github.com/joelkuiper/personograph'><i class='fab fa-github'></i></a>
5. **RGraphics** data and functions from the book 'R Graphics', second edition. [CRAN](https://cran.r-project.org/web/packages/RGraphics) <a href='https://www.stat.auckland.ac.nz/~paul/RG2e/index.html'><i class='fas fa-link'></i></a>
6. **tagcloud** generates tag and word clouds. [CRAN](https://cran.r-project.org/web/packages/tagcloud) <a href='https://github.com/ggobi/tourr/'><i class='fab fa-github'></i></a>
7. **tikzDevice** Provides a graphics output device for R that records plots in a LaTeX-friendly format. [CRAN](https://cran.r-project.org/web/packages/tikzDevice) <a href='https://github.com/yihui/tikzDevice'><i class='fab fa-github'></i></a>
8. **tourr** implements Tour methods in R code. [CRAN](https://cran.r-project.org/web/packages/tourr) <a href='https://github.com/ggobi/tourr/'><i class='fab fa-github'></i></a> <a href='https://doi.org/10.18637/jss.v040.i02'><i class='ai ai-doi'></i></a>
9. **wordcloud** creates word clouds. [CRAN](https://cran.r-project.org/web/packages/wordcloud)
10. **wordcloud2** R interface to wordcloud for data visualization. [CRAN](https://cran.r-project.org/web/packages/wordcloud2) <a href='https://github.com/Lchiffon/wordcloud2'><i class='fab fa-github'></i></a> <a href='https://timdream.org/wordcloud2.js/#love'><i class='fas fa-link'></i></a>
<br/> 

## Web-based interactive charts
1. **dygraphs** Interface to 'Dygraphs' interactive time series charting library. [CRAN](https://cran.r-project.org/web/packages/dygraphs) <a href='https://github.com/rstudio/dygraphs'><i class='fab fa-github'></i></a> <a href='https://rstudio.github.io/dygraphs/'><i class='fas fa-link'></i></a>
2. **heatmaply** Interactive Heat Maps Using 'plotly' [CRAN](https://cran.r-project.org/web/packages/heatmaply) <a href='https://github.com/talgalili/heatmaply'><i class='fab fa-github'></i></a>
3. **highcharter** R wrapper for highcharts. [CRAN](https://cran.r-project.org/web/packages/highcharter) <a href='https://github.com/jkunst.com/highcharter/'><i class='fab fa-github'></i></a> <a href='http://jkunst.com/highcharter/'><i class='fas fa-link'></i></a>
4. **htmlwidgets** a framework for easily creating R bindings to JavaScript libraries. [CRAN](https://cran.r-project.org/web/packages/htmlwidgets) <a href='https://github.com/ramnathv/htmlwidget'><i class='fab fa-github'></i></a> <a href='http://www.htmlwidgets.org'><i class='fas fa-link'></i></a>
5. **manhattanly** create interactive manhattan and Q-Q plots [CRAN](https://cran.r-project.org/web/packages/manhattanly) <a href='https://github.com/sahirbhatnagar/manhattanly'><i class='fab fa-github'></i></a>
6. **metricsgraphics** Creates interactive charts with the JavaScript 'MetricsGraphics' library. [CRAN](https://cran.r-project.org/web/packages/metricsgraphics) <a href='https://github.com/hrbrmstr/metricsgraphics'><i class='fab fa-github'></i></a> <a href='http://hrbrmstr.github.io/metricsgraphics/'><i class='fas fa-link'></i></a>
7. **networkD3** creates 'D3' 'JavaScript' network, tree, dendrogram, and Sankey graphs from 'R'. [CRAN](https://cran.r-project.org/web/packages/networkD3) <a href='https://github.com//christophergandrud/networkD3'><i class='fab fa-github'></i></a>
8. **plotly** translates 'ggplot2' graphs to an interactive web-based version and/or creates custom web-based visualizations directly from R. [CRAN](https://cran.r-project.org/web/packages/plotly) <a href='https://github.com//ropensci/plotly'><i class='fab fa-github'></i></a> <a href='https://plot.ly/r/'><i class='fas fa-link'></i></a>
9. **qtlcharts** Web-based interactive charts for the analysis of experimental crosses to identify genetic loci contributing to variation in quantitative traits. [CRAN](https://cran.r-project.org/web/packages/qtlcharts) <a href='https://github.com/kbroman/qtlcharts'><i class='fab fa-github'></i></a> <a href='http://kbroman.org/qtlcharts/'><i class='fas fa-link'></i></a>
10. **radarchart** create interactive radar charts using the 'Chart.js' JavaScript library and the 'htmlwidgets' package. [CRAN](https://cran.r-project.org/web/packages/radarchart) <a href='https://github.com/mangothecat/radarchart'><i class='fab fa-github'></i></a>
11. **rCharts (not available on CRAN)** creates, customizes and publishes interactive javascript visualizations from R using a familiar lattice style plotting interface. [CRAN](https://cran.r-project.org/web/packages/rCharts (not available on CRAN)) <a href='https://github.com/ramnathv/rCharts'><i class='fab fa-github'></i></a> <a href='http://rcharts.io'><i class='fas fa-link'></i></a>
12. **rbokeh** R interface for Bokeh which renders plots using HTML canvas and provides many mechanisms for interactivity. [CRAN](https://cran.r-project.org/web/packages/rbokeh) <a href='https://github.com/bokeh/rbokeh'><i class='fab fa-github'></i></a> <a href='http://hafen.github.io/rbokeh/'><i class='fas fa-link'></i></a>
13. **scatterD3** creates 'D3' 'JavaScript' scatterplots from 'R' with interactive features. [CRAN](https://cran.r-project.org/web/packages/scatterD3) <a href='https://github.com//juba/scatterD3'><i class='fab fa-github'></i></a> <a href='https://cran.r-project.org/web/packages/scatterD3/vignettes/introduction.html'><i class='fas fa-link'></i></a>
14. **shiny** web application framework for R. [CRAN](https://cran.r-project.org/web/packages/shiny) <a href='https://github.com/rstudio/shiny'><i class='fab fa-github'></i></a> <a href='http://shiny.rstudio.com'><i class='fas fa-link'></i></a>
15. **threeJS** create interactive 3D scatter plots, network plots, and globes using the 'three.js' visualization library. [CRAN](https://cran.r-project.org/web/packages/threeJS) <a href='https://github.com/bwlewis/rthreejs'><i class='fab fa-github'></i></a> <a href='http://bwlewis.github.io/rthreejs'><i class='fas fa-link'></i></a>
16. **manipulateWidget** add even more interactivity to interactive charts. [CRAN](https://cran.r-project.org/web/packages/manipulateWidget) <a href='https://github.com/rte-antares-rpackage/manipulateWidget'><i class='fab fa-github'></i></a>
<br/> 
