# First steps

In order to introduce new users quickly and concisely, we display a collection of the basic SpaceMath v1.0 commands for the Signal Strenghts with their application to the Two-Higgs-Doublet Model Type-III (THDM-III). There are common arguments in all $$\texttt{SpaceMath v1.0}$$ commands; for this reason, let us first list them in Table 2. While in Tables 3, 4, 5, 6, we display the main commands to generate plots and tables with allowed regions by the most up-to-date experimental results.

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

| Commands to generate {R}\_X graphs                                                                                                                                                                         |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| RVone\[ghtt\_,ghbb\_,ghVV\_,x\_,xmin\_,xmax\_,xlabel\_]\[\[i]]                                                                                                                                             |
| This command graphs $$\mathcal{R}_{V}$$ (V = W, Z) as a function of x.                                                                                                                                     |
| RGAMone\[ghtt\_,ghbb\_,ghWW\_,gCH\_,mCH\_,x\_,xmin\_,xmax\_,xlabel\_]\[\[i]]                                                                                                                               |
| This command graphs $$\mathcal{R}_{\gamma}$$ as a function of x.                                                                                                                                           |
| RTAUone\[ghtt\_, ghbb\_, ghtautau\_, x\_, xmin\_, xmax\_, xlabel\_]\[\[i]]                                                                                                                                 |
| This command graphs $$\mathcal{R}_{\tau}$$ as a function of x.                                                                                                                                             |
| RBOTone\[ghtt\_, ghbb\_, x\_, xmin\_, xmax\_, xlabel\_]\[\[i]]                                                                                                                                             |
| This command graphs $$\mathcal{R}_{b}$$ as a function of x.                                                                                                                                                |
| RV\[ghtt\_, ghbb\_, ghVV\_, x\_, y\_, xmin\_, xmax\_, ymin\_, ymax\_, xlabel\_, ylabel\_, xfor\_, yfor\_, xformin\_, xformax\_, xforstep\_, yformin\_, yformax\_, yforstep\_, PP\_]\[\[i]]                 |
| This command graphs $$\mathcal{R}_{V}$$ (V = W, Z) as a function of the parameters to be constrained: x, y, xfor, yfor.                                                                                    |
| RGam\[ghtt\_, ghbb\_, ghWW\_, gCH\_, mCH\_, x\_, y\_, xmin\_, xmax\_, ymin\_, ymax\_, xlabel\_, ylabel\_, xfor\_, yfor\_, xformin\_, xformax\_, xforstep\_, yformin\_, yformax\_, yforstep\_, PP\_]\[\[i]] |
| This command graphs $$\mathcal{R}_{\gamma}$$ as a function of the parameters to be constrained: x, y, xfor, yfor.                                                                                          |
| Rtau\[ghtt\_, ghbb\_, ghtautau\_, x\_, y\_, xmin\_, xmax\_, ymin\_, ymax\_, xlabel\_, ylabel\_, xfor\_, yfor\_, xformin\_, xformax\_, xforstep\_, yformin\_, yformax\_, yforstep\_, PP\_] \[\[i]]          |
| This command graphs $$\mathcal{R}_{\tau}$$ as a function of the parameters to be constrained: x, y, xfor, yfor.                                                                                            |
| Rb\[ghtt\_, ghbb\_, x\_, y\_, xmin\_, xmax\_, ymin\_, ymax\_, xlabel\_, ylabel\_, xfor\_, yfor\_, xformin\_, xformax\_, xforstep\_, yformin\_, yformax\_, yforstep\_, PP\_]\[\[i]]                         |
| This command graphs $$\mathcal{R}_{b}$$ as a function of the parameters to be constrained: x, y, xfor, yfor.                                                                                               |



| Commands to generate random values for \mathcal{R}\_X.                                                                                                  |
| ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| RVRandom\[ghtt\_, ghbb\_, ghVV\_, x1\_, x1min\_, x1max\_, x2\_, x2min\_, x2max\_, x3\_, x3min\_, x3max\_, x4\_, x4min\_, x4max\_, NN\_ ]                |
| This command generates random values that satisfy the experimental constraint on $$\mathcal{R}_{V}$$.                                                   |
| PlotRVRandom\[ci\_, cj\_, xlabel\_, ylabel\_ ]\[\[i]]                                                                                                   |
| This command graphs the plane ci-cj once RVRandom was executed.                                                                                         |
| RgamRandom\[ghtt\_, ghbb\_, ghWW\_, gCH\_, mCH\_, x1\_, x1min\_, x1max\_, x2\_, x2min\_, x2max\_, x3\_, x3min\_, x3max\_, x4\_, x4min\_, x4max\_, NN\_] |
| This command generates random values that satisfy the experimental constraint on $$\mathcal{R}_{\gamma}$$.                                              |
| PlotRgamRandom\[ci\_, cj\_, xlabel\_, ylabel\_ ]\[\[i]]                                                                                                 |
| This command graphs the plane ci-cj once RgamRandom was executed.                                                                                       |
| RtauRandom\[ghtt\_, ghbb\_, ghtautau\_, x1\_, x1min\_, x1max\_, x2\_, x2min\_, x2max\_, x3\_, x3min\_, x3max\_, x4\_, x4min\_, x4max\_, NN\_]           |
| This command generates random values that satisfy the experimental constraint on $$\mathcal{R}_{\tau}$$.                                                |
| PlotRtauRandom\[ci\_, cj\_, xlabel\_, ylabel\_ ]\[\[i]]                                                                                                 |
| This command graphs the plane ci-cj once RtauRandom was executed.                                                                                       |
| RbRandom\[ghtt\_, ghbb\_, x1\_, x1min\_, x1max\_, x2\_, x2min\_, x2max\_, x3\_, x3min\_, x3max\_, x4\_, x4min\_, x4max\_, NN\_ ]                        |
| This command generates random values that satisfy the experimental constraint on $$\mathcal{R}_{b}$$.                                                   |
| PlotRbRandom\[ci\_, cj\_, xlabel\_, ylabel\_ ]\[\[i]]                                                                                                   |
| This command graphs the plane ci-cj once RbRandom was executed.                                                                                         |



| Commands for generate tables of \mathcal{R}\_X's.                                                                                                                                        |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| TableRVone\[ghtt\_, ghbb\_, ghVV\_, x\_, xmin\_, xmax\_, xstep\_ ]                                                                                                                       |
| This command generates a table with two columns: RVone-x. The output file will be saved as TableRVone\_1sigma.txt and TableRVone\_2sigma.txt in $UserDocumentsDirectory. Here V = W, Z.  |
| TableRGAMone\[ghtt\_, ghbb\_, ghWW\_, gCH\_, mCH\_, x\_, xmin\_, xmax\_, xstep\_ ]                                                                                                       |
| This command generates a table with two columns: RGAMone-x. The output file will be saved as TableRGAMone\_1sigma.txt and TableRGAMone\_2sigma.txt in $UserDocumentsDirectory.           |
| TableRTAUone\[ghtt\_, ghbb\_, ghtautau\_, x\_, xmin\_, xmax\_, xstep\_ ]                                                                                                                 |
| This command generates a table with two columns: RTAUone-x. The output file will be saved as TableRTAUone\_1sigma.txt and TableRTAUone\_2sigma.txt in $UserDocumentsDirectory.           |
| TableRBOTone\[ghtt\_, ghbb\_, x\_, xmin\_, xmax\_, xstep\_ ]                                                                                                                             |
| This command generates a table with two columns: RBOTone-x. The output file will be saved as TableRBOTone\_1sigma.txt and TableRBOTone\_2sigma.txt in $UserDocumentsDirectory.           |
| TableRV\[ghtt\_, ghbb\_, ghVV\_, x\_, xmin\_, xmax\_, xstep\_, y\_, ymin\_, ymax\_, ystep\_ ]                                                                                            |
| This command generates a table with three entries arranged as {RV, x, y}, The output file will be saved as TableRV\_1sigma.txt and TableRV\_2sigma.txt in $UserDocumentsDirectory.       |
| TableRGam\[ghtt\_, ghbb\_, ghWW\_, gCH\_, mCH\_, x\_, xmin\_, xmax\_, xstep\_, y\_, ymin\_, ymax\_, ystep\_ ]                                                                            |
| This command generates a table with three entries arranged as {RGam, x, y}, The output file will be saved as TableRgam\_1sigma.txt and TableRgam\_2sigma.txt in $UserDocumentsDirectory. |
| TableRb\[ghtt\_, ghbb\_, x\_, xmin\_, xmax\_, xstep\_, y\_, ymin\_, ymax\_, ystep\_]                                                                                                     |
| This command generates a table with three entries arranged as {RV, x, y}, The output file will be saved as TableRb\_1sigma.txt and TableRb\_2sigma.txt in $UserDocumentsDirectory.       |
| TableRtau\[ghtt\_, ghbb\_, ghtautau\_, x\_, xmin\_, xmax\_, xstep\_, y\_, ymin\_, ymax\_, ystep\_]                                                                                       |
| This command generates a table with three entries arranged as {Rtau, x, y}, The output file will be saved as TableRtau\_1sigma.txt and TableRtau\_2sigma.txt in $UserDocumentsDirectory. |



| Commands to generate R\_X graphs.                                                                                                                                                                                                         |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| RXALL\[ghtt\_, ghbb\_, ghZZ\_, ghWW\_, ghtautau\_, gCH\_, mCH\_, x\_, y\_, xmin\_, xmax\_, ymin\_, ymax\_, xlabel\_, ylabel\_, xfor\_, yfor\_, xformin\_, xformax\_, xforstep\_, yformin\_, yformax\_, yforstep\_, PP\_ ]\[\[i]]          |
| This command graphs all signal strengths in a same plot as a function of x, y, xfor, yfor.                                                                                                                                                |
| RXintersection\[ghtt\_, ghbb\_, ghZZ\_, ghWW\_, ghtautau\_, gCH\_, mCH\_, x\_, y\_, xmin\_, xmax\_, ymin\_, ymax\_, xlabel\_, ylabel\_, xfor\_, yfor\_, xformin\_, xformax\_, xforstep\_, yformin\_, yformax\_, yforstep\_, PP\_ ]\[\[i]] |
| This command graphs the intersection of all signal strengths, if any.                                                                                                                                                                     |

{% embed url="https://wolfram.com/xid/0v5uff33qdhdq-bmjevd" %}

