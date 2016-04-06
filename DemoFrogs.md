_This example includes the use of marginal.plot, groups, splom, spatial point data, and the z variable for a 3D point-cloud._

The `frogs` dataset is available in the **DAAG** package. The data are on the distribution of the Southern Corroboree frog, which occurs in the Snowy Mountains area of New South Wales, Australia.

```
library(DAAG)
latticist(frogs)
```

![http://playwith.googlecode.com/files/latticistFrogs_A_01.png](http://playwith.googlecode.com/files/latticistFrogs_A_01.png)

The initial display shows marginal distributions of all variables in the data frame. The x axis labels give a summary of the range of each variable. Begin by clicking "choose variables" and reducing the number of variables shown:

![http://playwith.googlecode.com/files/latticistFrogs_B_01.png](http://playwith.googlecode.com/files/latticistFrogs_B_01.png)

Now, with a more manageable number of variables, set the "groups" to `pres.abs`, which indicates whether frogs were present (1) or absent (0) at each location.

![http://playwith.googlecode.com/files/latticistFrogs_C_01.png](http://playwith.googlecode.com/files/latticistFrogs_C_01.png)

This reveals relationships with distance, number of sites, and temperature (maybe the frogs find it too cold below 2 degrees C).

![http://playwith.googlecode.com/files/latticistFrogs_D_01.png](http://playwith.googlecode.com/files/latticistFrogs_D_01.png)

Click the "splom" button in the Hypervariate section to convert the display to a scatter-plot matrix. The groups are not very helpful here, but there are obvious correlations between altitude, temperature and, to a lesser degree, rainfall.

![http://playwith.googlecode.com/files/latticistFrogs_E_01.png](http://playwith.googlecode.com/files/latticistFrogs_E_01.png)

To view the spatial distribution of observations, set the x and y variables to "easting" and "northing":

![http://playwith.googlecode.com/files/latticistFrogs_F_01.png](http://playwith.googlecode.com/files/latticistFrogs_F_01.png)

The lines here come from a _loess_ smoother, which treats the y variable as a function of the x variable; that is not appropriate in this case, so remove them by clicking the "Lines" checkbox. Also set the "Aspect" option to "iso", because x and y are in the same units.

![http://playwith.googlecode.com/files/latticistFrogs_G_02.png](http://playwith.googlecode.com/files/latticistFrogs_G_02.png)

Set the z variable to "altitude". The 3D view can be rotated and zoomed.

![http://playwith.googlecode.com/files/latticistFrogs_H_01.png](http://playwith.googlecode.com/files/latticistFrogs_H_01.png)

From this view it appears that the frog populations are clustered on the slopes in distinct valleys. Only a few outlying sites in the higher land support populations.

![http://playwith.googlecode.com/files/latticistFrogs_I_01.png](http://playwith.googlecode.com/files/latticistFrogs_I_01.png)

Right-click on a point to see the values of all variables. (It is also possible to add a persistent label this way).

![http://playwith.googlecode.com/files/latticistFrogs_J_01.png](http://playwith.googlecode.com/files/latticistFrogs_J_01.png)