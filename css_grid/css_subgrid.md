# 🔥CSS SubGrid

?> When you add **display: grid** to a grid container, only the direct children become grid items and can then be placed on the grid that you have created. The children of these items display in normal flow.

?> You can **"nest" grids by making a grid item a grid container**. These grids however are independent of the parent grid and of each other, meaning that they do not take their track sizing from the parent grid. This makes it difficult to line nested grid items up with the main grid.

?> If you set the value **subgrid** on **grid-template-columns, grid-template-rows** or both, instead of creating a new track listing the nested grid uses the tracks defined on the parent.

> [🌐 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout/Subgrid)