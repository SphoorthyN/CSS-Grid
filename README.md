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
1. ***Finished layout***

    ![Layout 1](assets/README/layout_1/Inner&#32;grid.png) 

------
1. ***Outer grid***
  
        .container
            grid-template-rows: repeat(7, 1fr)
            grid-template-columns: repeat(4, 1fr)

    ![Outer grid](assets/README/layout_1/Outer&#32;grid.png)

    You can see slight mismatches between the 3 small boxes, the big box under it and the grid lines since they're laid out to another grid defined as below.

    This happens since the vertical sidebar isn't in the same-sized column as the one defined in the *outer grid*. It is in fact *0.9fr* rather than the *1fr* column shown in the above image. 
    
    There's no reason for this other than the fact that I wanted that sidebar to be slightly smaller in width than the individual boxes.

------
1. ***Inner grid*** 
  
        .container
            main
                article
                    grid-template-columns: repeat(3, 1fr) .9fr
                    grid-template-rows: repeat(4, 1fr)

    ![Inner grid](assets/README/layout_1/Inner&#32;grid.png)

    As you can see here, the grid lines match up perfectly, as they should, since they've been placed in the cells. *Duh*.

    This grid is not the exact same as the *outer grid*. The way I see it is, the *1fr* columns I've defined here aren't the same as the *1fr* columns defined in the *outer grid*. 
    
    This is due to the fact that the first three columns in the *inner grid* shown above have more width to fill than the first three columns of the *outer grid* since the fourth column of the *inner grid* is *0.9fr* units wide, which is thinner than the *1fr* wide fourth column of the *outer grid*.