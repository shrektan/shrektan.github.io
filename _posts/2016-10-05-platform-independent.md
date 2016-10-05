> It's easier to say than to do. 

Although __R__ is designed to be platform independent, it's not that simple to achieve that. 99% is ok but there're always the rest 1% part costs you days to struggle.

Recently, I'm trying to build an R project which intends to be used in an offline computer. I'm making the project in my macbook pro. So there're two things left to be done:

1. Make sure there's no surprise on windows,
1. Find a way install the R packages in an offline PC, considering the dependencies of these packages.

For the 1st issue, what I'm doing is to aviod the potential encoding issues as well as the timezone issues. Specifically:

1. always write to UTF-8 encoding, and set the reading encoding param properly,
1. avoid non-ASCII chars to be the key in `data.table`,
1. always write to UTC timezone and show in PRC timezone

For the 2nd issue, things are getting harder. After some exploring, I thought `packrat` would be ideal for this, right? [`Packrat`](http://rstudio.github.io/packrat/) is a R package denpendence management system, developped by Rstudio. It could automatically record the packages that used in your package and storage their source files. Sound perfect, right? Since the _source files_ of the packages have been storaged in the folder and we can easily build the packages from source files, right?

It turns out there're a few packages need to download from external files, even they're on CRAN. For example, `curl` needs `libcurl` library for windows and `stringi` is even more complicated. 

And it seems like the only way to do is to maintain a CRAN liked local repo, like [shrekran](https://github.com/shrektan/shrekran), to storage these binary libraries of windows.

`miniCRAN` might be a solution, but more issues need to take consideration. 

I'll update this post when I figure out my way. 
