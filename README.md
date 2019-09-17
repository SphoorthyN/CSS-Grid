# CSS GRID Practice Exercises and Examples


This is a collection of different layouts using CSS grids, both complex and trivial, practice assignments, self-developed layouts as well as my interpretation of different layouts from print media as I keep learning how to use CSS Grids. 

I will try to document each layout as well as I can, but I'm a naturally messy person, so fingers crossed.

> **Note:** Wherever possible, I've linked the related files. For example, the heading *Layout_1* takes you to the *layout_1.html* file of the same repository.

------

#### 1. [Layout_1](html/layout_1.html)

> The SASS stylesheets for this layout are **[HERE](assets/layout_1/layout_1.sass)**. 
> 
> In case you want to see the compiled CSS stylesheets, click **[HERE](assets/layout_1/layout_1.css)**.

A simple layout, where I nested a grid inside the main grid. 

![Layout 1](assets/README/layout_1/layout_1.png) ***Finished layout***


------

![Outer grid](assets/README/layout_1/Outer&#32;grid.png) ***Outer grid  | .container***


**grid-template-rows:** repeat(7, 1fr)


**grid-template-columns:** repeat(4, 1fr)

<br>
---
<br>

![Inner grid](assets/README/layout_1/Inner&#32;grid.png) ***Inner grid | .container > main > article***

**grid-template-columns:** repeat(3, 1fr) 0.9fr

**grid-template-rows:**  repeat(4, 1fr)
