---
title: Pull Request Workflow Example
author: Data Carpentry contributors
teaching: 5
exercises: 10
editor_options:
  chunk_output_type: console
---


We will use the code block and output below to demonstrate one of the new features
provided by The Carpentries Workbench: automated feedback about changes to the
rendered lesson content that would be made by a pull request.


```r
pie(
  c(Sky = 78, "Sunny side of pyramid" = 17, "Shady side of pyramid" = 5), 
  init.angle = 315, 
  col = c("deepskyblue", "yellow", "yellow3"), 
  border = FALSE
)
```

<div class="figure" style="text-align: center">
<img src="fig/06-pyramid-example-rendered-pyramid-1.png" alt="pie chart illusion of a pyramid"  />
<p class="caption">Sun arise each and every morning</p>
</div>

::: challenge

#### Change the colour of the pyramid

1. Fork this repository
1. Find the source RMarkdown file for this episode in your fork
1. Change the colours of the pyramid parts of the figure above 
   (defined in the `col` parameter of `pie`). Here is a [resource for the available colour names in R](https://r-charts.com/colors/)
1. Commit the change
1. Open a pull request to https://github.com/fishtree-attempt/R-ecology-lesson/ 
   based on the change you made
1. Look at the preview of the changes to rendered content. 
   This should appear as a comment in the pull request discussion tab 
   shortly after the PR has been opened.

:::::: solution


```r
pie(
  c(Sky = 78, "Sunny side of pyramid" = 17, "Shady side of pyramid" = 5), 
  init.angle = 315, 
  col = c("deepskyblue", "palegreen", "limegreen"), 
  border = FALSE
)
```

<div class="figure" style="text-align: center">
<img src="fig/06-pyramid-example-rendered-pyramid-green-1.png" alt="pie chart illusion of a pyramid"  />
<p class="caption">Sun arise each and every morning</p>
</div>

::::::
:::
