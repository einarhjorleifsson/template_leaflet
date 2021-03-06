# template_leaflet

## From here onwards

    git clone https://github.com/einarhjorleifsson/template_leaflet.git
    mv template_leaflet your_title
    cd your_title
    rm -rf .git
    git init
    
From here on one can customize the 'section0*.Rmd' files to ones own needs and then 'knit' the stuff.


## How did I get here?

    git clone git@github.com:rstudio/leaflet.git template_leaflet
    cd template_leaflet/
    git checkout gh-pages
    rm -rf .git
    rm -r colors_files
    rm -r images
    rm -r json
    rm -r nc
    rm -r shp
    rm *.html
    mv map_widget.Rmd section01.Rmd

some manual editing on index.Rmd section01.Rmd

    cp section01.Rmd section02.Rmd
    cp section01.Rmd section03.Rmd
    cp section01.Rmd section04.Rmd
    cp section01.Rmd section05.Rmd
    cp section01.Rmd section06.Rmd
    cp section01.Rmd section07.Rmd
    
    rm basemaps.Rmd
    rm colors.Rmd
    rm json.Rmd
    rm legends.Rmd
    rm markers.Rmd
    rm popups.Rmd
    rm raster.Rmd
    rm scratch.Rmd
    rm shapes.Rmd
    rm shiny.Rmd
    rm showhide.Rmd
    
    
some manual editing on section*.Rmd files

Edited '_includes/before_body.html'

Among other things:

```
    <div class="list-group">
      <a class="list-group-item" href="./">Introduction</a>
      <a class="list-group-item" href="section01.html">section 1</a>
      <a class="list-group-item" href="section02.html">section 2</a>
      <a class="list-group-item" href="section03.html">section 3</a>
      <a class="list-group-item" href="section04.html">section 4</a>
      <a class="list-group-item" href="section05.html">section 5</a>
      <a class="list-group-item" href="section06.html">section 6</a>
      <a class="list-group-item" href="section07.html">section 7</a>
    </div>
```

Edited '_includes/after_body.html'

    rm -r libs/leaflet*
    rm -r libs/h*
    rm -r libs/j
    
    git add *
    git add .gitignore
    git add .nojekyll

    git remote add origin git@github.com:einarhjorleifsson/template_leaflet.git
    git commit -m 'seeding'
    git push -u origin master
