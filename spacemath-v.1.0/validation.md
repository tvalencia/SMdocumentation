# Validation

In order to validate SpaceMath v1.0, we apply the coupling modifiers $$\kappa_i$$ defined in eq. \eqref{kappas} to the Two-Higgs Doublet Model of Type I and II (THDM-I, II). In Ref. \cite{Craig:2012vn} are reported $$\kappa_b$$ and $$\kappa_V$$ in the context of these models. To reproduce these results via \texttt{SpaceMath} v1.0 the only thing we need is to know the model couplings, which are given in Table \ref{AcoplosTHDM}. The commands to evaluate $$\kappa_b$$ and $$\kappa_V$$ are displayed in Table \ref{commadKbkV}.

| Coupling                                                                            | Input to SpaceMath                                        |  Command \kappa\_i                           |
| ----------------------------------------------------------------------------------- | --------------------------------------------------------- | -------------------------------------------- |
| $$g_{hbb}^{THDM-I}=\frac{gm_{b}}{2m_{W}}\left(\frac{\cos\alpha}{\sin\beta}\right)$$ | $$ghbb[Sa\_,Tb\_,Cb\_]:=g*mb*Sqrt[1-Sa ^2]/(2*mW*Tb*Cb)$$ | $$kb[\texttt{ghbb[Sa,Tb,Cos[ArcTan[Tb]]}]]$$ |
|                                                                                     |                                                           |                                              |
|                                                                                     |                                                           |                                              |
