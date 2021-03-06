---
categories:
- R
- RMarkdown
date: "2020-07-20"
tags:
- R Markdown
#thumbnailImage: //d1u9biwaxjngwg.cloudfront.net/highlighted-code-showcase/peak-140.jpg
#thumbnailImagePosition: left
title: R Markdown
---

 

This post shows how to format your RMarkdown. Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>.
<!--more-->


# Markdown

{{< codeblock "Rmarkdown.md" "md" "http://underscorejs.org/#compact" "Rmarkdown.md" >}}

Headings 
------------------------------------
# first level heading

## second level heading

### third level heading

Inline text formatting
------------------------------------
**Bold** 

*italic* or _italic_

superscript^2^ or superscript H^3^P0~4~

Links and images
-------------------------------------

links [RStudio](https://www.rstudio.com)

images ![image title](pathtoimage)

inline link with reference [link references][1].
    [1]: http://example.com

footnote ^[footnote]

Lists
--------------------------------------
# Unordered items
- unordered item 1
- two
    - sub-one
    - sub-two
    
# Ordered or numbered items 
1. ordered item 1
2. two
    1. sub-one
    2. sub-two

Tables 
-----------------------------------------

First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

Blockquotes
---------------------------------------
> "some text"
>
> --- Mitul Patel


Code
----------------------------------------
inline code `r 1+2`
code chunk ```{r} 1+2```
{{< /codeblock >}}

Also you can also indent the blocks by four spaces.

## Code Chunk options
Chunk output can be customised with options, arguments needs to be supplied to chunk header. We will look at most important set of options below, but you an access [full list](http://yihui.name/knitr/options/) for more options. 

`eval = FALSE` prevents code from being evaluated, so obviously no results will be generated.

`include = FALSE` runs the code, but doesn’t show the code or results in the final document.

`echo = FALSE` prevents code, but not the results from appearing in the finished file. 

`message = FALSE` or `warning = FALSE` prevents messages or warnings from appearing in the finished file.

`results = 'hide'` hides printed output; 

`fig.show = 'hide'` hides plots.

`error = TRUE` causes the render to continue even if code returns an error. 

`collapse =TRUE` to merge text output and source code into a single code block in the output.
