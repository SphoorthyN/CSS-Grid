# CSS GRID Practice Exercises and Examples


This is a collection of different layouts using CSS grids, both complex and trivial, practice assignments, self-developed layouts as well as my interpretation of different layouts from print media as I keep learning how to use CSS Grids. 

I will try to document each layout as well as I can, but I'm a naturally messy person, so fingers crossed.

------

#### 1. Layout_1
A simple layout, where I nested a grid inside the main grid. 

![Layout 1](assets/README/layout_1/layout_1.png) ***Finished layout***

<br>
---
<br>

![Outer grid](assets/README/layout_1/Outer&#32;grid.png) ***Outer grid  | .container***


**grid-template-rows:** repeat(7, 1fr)


**grid-template-columns:** repeat(4, 1fr)

<br>
---
<br>

![Inner grid](assets/README/layout_1/Inner&#32;grid.png) ***Inner grid | .container > main > article***

**grid-template-columns:** repeat(3, 1fr) 0.9fr

**grid-template-rows:**  repeat(4, 1fr)
