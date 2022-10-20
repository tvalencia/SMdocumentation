# First steps

| Argument          | Description                                                                                                                                                                                                      |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ghtt              | Coupling of the Higgs boson to a top quark pair.                                                                                                                                                                 |
| ghbb              | Coupling of the Higgs boson to a bottom quark pair.                                                                                                                                                              |
| ghtautau          | Coupling of the Higgs boson to a $$\tau$$ lepton pair.                                                                                                                                                           |
| ghVV              | Coupling of the Higgs boson to a _V=W, Z_ gauge boson pair.                                                                                                                                                      |
| gCH               | Coupling of the Higgs boson to a charged scalar boson pair.                                                                                                                                                      |
| x, y, xfor, yfor  | Parameters to constrain.                                                                                                                                                                                         |
| xmin, xmax        | Interval from xmin to xmax for parameter x: xmin$$\leq$$​x $$\leq$$ xmax.                                                                                                                                        |
| ymin, ymax        | Interval from ymin to ymax for parameter y: ymin$$\leq$$y$$\leq$$ymax.                                                                                                                                           |
| xformin, xformax  | <p>Interval from xformin to xformax for parameter xfor: </p><p>xformin<span class="math">\leq</span>xfor<span class="math">\leq</span>xformax.</p>                                                               |
| yformin, yformax  | Interval from yformin to yformax for parameter yfor: yformin$$\leq$$yfor$$\leq$$yformax.                                                                                                                         |
| xforstep          | Steps from xformin to xformax.                                                                                                                                                                                   |
| yforstep          | Steps from yformin to yformax.                                                                                                                                                                                   |
| xlabel (ylabel)   | Label for x axis (y axis).                                                                                                                                                                                       |
| PP                | Sample points to use for plotting functions. We suggest to consider values until PP=100 and for PP>100 High-Performance Computing is recommend,  or you can use our server, see Appx. \ref{cluster} for details. |
| NN                | Number of random values to generate.                                                                                                                                                                             |
| \[\[i]]           | Stands for confidence level i=1 (2), indicates 1$$\sigma$$ (2$$\sigma$$).                                                                                                                                        |
| mCH               | Charged scalar mass.                                                                                                                                                                                             |
| xi, i=1, 2, 3, 4. | Random values parameters to be generated.                                                                                                                                                                        |

| Commands to generate {R}\_X graphs                                           |
| ---------------------------------------------------------------------------- |
| RVone\[ghtt\_,ghbb\_,ghVV\_,x\_,xmin\_,xmax\_,xlabel\_]\[\[i]]               |
| This command graphs $$\mathcal{R}_{V}$$ (V = W, Z) as a function of x.       |
| RGAMone\[ghtt\_,ghbb\_,ghWW\_,gCH\_,mCH\_,x\_,xmin\_,xmax\_,xlabel\_]\[\[i]] |
| This command graphs $$\mathcal{R}_{\gamma}$$ as a function of x.             |
| RTAUone\[ghtt\_, ghbb\_, ghtautau\_, x\_, xmin\_, xmax\_, xlabel\_]\[\[i]]   |
|                                                                              |
