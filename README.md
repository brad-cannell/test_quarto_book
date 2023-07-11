# Test Quarto Book

This repository is just for testing out [Quarto book](https://quarto.org/docs/books/) development. For now, I'm just using it for some experimentation.

This is **not** my new R Notes book; although, I may move R Notes over to Quarto at some point. This is purely just a sandbox for playing with Quarto books.

## Useful websites:

-   [Quarto book documentation](https://quarto.org/docs/books/)

## Rendering

We can render the files by clicking the Render button in RStudio. To render the HTML and PDF files at the same time, type `quarto render` into the terminal. 

````
```{bash}
quarto render
```
````

You can also render Quarto files with a native R code chunk.

- The input argument: The input file or project directory to be rendered (defaults to rendering the project in the current working directory).

- The output_format argument: Target output format (defaults to "html"). The option "all" will render all formats defined within the file or project.

````
```{r}
#| Render with R
#| eval: false
quarto::quarto_render(output_format = "all")
```
````

## Publishing to GitHub pages

[This article is great](https://quarto.org/docs/publishing/github-pages.html). After committing, and making sure you are on the main branch, type `quarto publish gh-pages` in the terminal.

````
```{bash}
quarto publish gh-pages
```
````


## Publishing to Netlify

[This article is great](https://quarto.org/docs/publishing/netlify.html). After committing, and making sure you are on the main branch, type `quarto publish netlify` in the terminal.

````
```{bash}
quarto publish netlify
```
````

## Where to publish

I've used Netlify in the past and have been happy with it. However, I'm not sure that it is necessary or efficient to add the extra layer of using Netlify in GitHub Pages will work just as well. Why introduce a third site into the mix if we don't have to? For now, I may just stick with GitHub Pages.
