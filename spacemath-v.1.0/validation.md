# Validation

In order to validate SpaceMath v1.0, we apply the coupling modifiers $$\kappa_i$$ defined in eq. \eqref{kappas} to the Two-Higgs Doublet Model of Type I and II (THDM-I, II). In Ref. \cite{Craig:2012vn} are reported $$\kappa_b$$ and $$\kappa_V$$ in the context of these models. To reproduce these results via \texttt{SpaceMath} v1.0 the only thing we need is to know the model couplings, which are given in Table \ref{AcoplosTHDM}. The commands to evaluate $$\kappa_b$$ and $$\kappa_V$$ are displayed in Table \ref{commadKbkV}.

| Coupling                                                                              | Input to SpaceMath                                                                               |  Command \kappa\_i                                              |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ | --------------------------------------------------------------- |
| $$g_{hbb}^{THDM-I}=\frac{gm_{b}}{2m_{W}}\left(\frac{\cos\alpha}{\sin\beta}\right)$$   | $$\texttt{ghbb[Sa\_,Tb\_,Cb\_]:=g*mb*Sqrt[1-Sa\textasciicircum2]/(2*mW*Tb*Cb)}$$                 | $$\texttt{kb[\texttt{ghbb[Sa,Tb,Cos[ArcTan[Tb]]}]]}$$           |
| $$g_{hbb}^{THDM-II}=\frac{gm_{b}}{2m_{W}}\left(\frac{-\sin\alpha}{\cos\beta}\right)$$ | $$\texttt{ghbb[Sa\_,Tb\_,Sb\_]:=-g*mb*Sa*Tb/(2*mW*Sb) }$$                                        | $$\texttt{kb[\texttt{ghbb[Sa,Tb,Sin[ArcTan[Tb]]}]]}$$           |
| $$g_{hVV}^{THDM-I,-II}=g_{V}m_{V}\sin(\beta-\alpha)$$                                 | $$\textrm{ghVV[Tb\_,Cb\_,Sb\_,Sa\_]:=((Tb*Cb*Sqrt[1-Sa\textasciicircum2])-(Sb/Tb*Sa))*(gv*mV)}$$ | $$\texttt{kV[ghVV[Tb, Cos[ArcTan[Tb]], Sin[ArcTan[Tb]], Sa]]}$$ |

