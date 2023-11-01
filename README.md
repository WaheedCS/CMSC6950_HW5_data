For each problem, the data is given in an `.npz` file.  You can load these files by running
```
import numpy as np
npzfile = np.load("iterations.npz")
```

To view a list of the data in the file, run
```
npzfile.files
```
To access the data array with name `my_name`, use `npzfile['my_name']`.


(a) (5 points) File `iterations.npz` contains a single array, `iteration_counts`, with iteration counts to solution for a particular algorithm applied to a set of 150 problems.  Plot this as a histogram, including a kernel density estimate.

(b) (10 points) File `heights.npz` contains 2D arrays of data describing the height of water at 4 times ($t = 0.25$, $0.5$, $0.75$, and $1.0$) from simulations of the shallow water equations.  Plot this data as a series of heat maps.  If helpful, the (x,y)$ coordinates of the simulation mesh are stored as arrays `X` and `Y` in the data file.

(c) (15 points) File `RR_data.npz` contains outputs of a quantity known as the reconnection rate from simulations run at 3 different Reynolds numbers (5000, 10000, 20000) and 4 different grid resolutions (denoted by `nref4`, `nref5`, `nref6`, and `nref7`).  For each Reynolds number and grid resolution, a single value is output and stored in an array (so that `RR10000_nref6` contains data for Reynolds number 10000 and refinement level 6) for each time value in the corresponding `times` array (`times_nref6` for `RR10000_nref6`).  Plot this data in a suitable set of line graphs, demonstrating convergence of the reconnection rate with resolution for each Reynolds number.

