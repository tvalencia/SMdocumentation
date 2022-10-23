# Constraint on free model parameter space of the THDM-III by using SpaceMath v1.0

We now turn to constrain the free model parameter space of the THDM-III focusing on the Yukawa interactions. As previously we mentioned, in SpaceMath v1.0 only the Higgs boson data are enabled. Then, we use signal strengths to find allowed regions which are in accordance with the most up-to-date experimental reports. We give, step by step, instructions on how SpaceMath v1.0 works. For enthusiastic users go to the Sec. \ref{impacientes}.

We first present an overview of the THDM-III focusing only on the details relevant of the Yukawa Lagrangian. For a detailed account of this model and the study of its phenomenology we refer the readers to Refs. \cite{Branco:2011iw, Botella:2009pq, Botella:2015hoa, Arroyo:2013tna, Cruz:2019vuo, HernandezSanchez:2012eg, BarradasGuevara:2010xs, Arroyo-Urena:2015uoa, GomezBock:2005hc, HernandezSanchez:2010zz, Arroyo-Urena:2019qhl, Arroyo-Urena:2020mgg}.

The most general $$SU(2)_L\times U(1)_Y$$ invariant scalar potential is given by \cite{Gunion:2002zf, Morettietal}:

$$
V(\Phi_{1},\Phi_{2})=\mu_{1}^{2}(\Phi_{1}^{\dagger}\Phi_{1})+\mu_{2}^{2}(\Phi_{2}^{\dagger}\Phi_{2})-\left(\mu_{12}^{2}(\Phi_{1}^{\dagger}\Phi_{2})+H.c.\right)+\frac{1}{2}\lambda_{1}(\Phi_{1}^{\dagger}\Phi_{1})^{2}
$$

$$
+\frac{1}{2}\lambda_{2}(\Phi_{2}^{\dagger}\Phi_{2})^{2}+\lambda_{3}(\Phi_{1}^{\dagger}\Phi_{1})(\Phi_{2}^{\dagger}\Phi_{2})+\lambda_{4}(\Phi_{1}^{\dagger}\Phi_{2})(\Phi_{2}^{\dagger}\Phi_{1})
$$

$$
+\left(\frac{1}{2}\lambda_{5}(\Phi_{1}^{\dagger}\Phi_{2})^{2}+\left(\lambda_{6}(\Phi_{1}^{\dagger}\Phi_{1})+\lambda_{7}(\Phi_{2}^{\dagger}\Phi_{2})\right)(\Phi_{1}^{\dagger}\Phi_{2})+H.c.\right),
$$

where $$\mu_{1, 2}$$, $$\lambda_{1, 2, 3 ,4}$$ are real parameters while $$\mu_{12}$$, $$\lambda_{5, 6, 7}$$ can be complex in general. The doublets are written as $$\Phi_{a}^T=\left( \phi_{a}^{+}, \phi_{a}^0\right)$$ for $$a=1, 2$$. After the Spontaneous Symmetry Breaking (SSB) the two Higgs doublets acquire non-zero expectation values. The Vacuum Expectation Values (VEV) are selected as

$$
\langle\Phi_{a}\rangle=\frac{1}{\sqrt{2}}\left(\begin{array}{c}
0\\
\upsilon_{a}
\end{array}\right),\,a=1,\,2
$$

where $$\upsilon_1$$ and $$\upsilon_2$$ satisfy $$\upsilon_1^2 + \upsilon_2^2 = \upsilon^2$$ for $$\upsilon=246$$ GeV.

In the most general case both doublets can participate in the interactions with the fermion fields. The Yukawa Lagrangian is written as

$$
\mathcal{L}_{Y}=Y_{1}^{u}\bar{Q}_{L}^{'}\tilde{\Phi}_{1}u_{R}^{'}+Y_{2}^{u}\bar{Q}_{L}^{'}\tilde{\Phi}_{2}u_{R}^{'}+Y_{1}^{d}\bar{Q}_{L}^{'}\Phi_{1}d_{R}^{'}
$$

$$
+Y_{2}^{d}\bar{Q}_{L}^{'}\Phi_{2}d_{R}^{'}+Y_{1}^{\ell}\bar{L}_{L}^{'}\Phi_{1}\ell_{R}^{'}+Y_{2}^{\ell}\bar{L}_{L}^{'}\Phi_{2}\ell_{R}^{'}+H.c.,
$$

Because we are interested in neutral interactions we only present the neutral part of the Yukawa Lagrangian of Eq. \eqref{Yukawa} which reads: \cite{Arroyo:2013tna}

$$
\mathcal{L}_{Y}^{N}=Y_{1}^{u}\bar{Q}_{L}^{0}\tilde{\Phi}_{1}u_{R}^{0}+Y_{2}^{u}\bar{Q}_{L}^{0}\tilde{\Phi}_{2}u_{R}^{0}+Y_{1}^{d}\bar{Q}_{L}^{0}\Phi_{1}d_{R}^{0}
$$

$$
+Y_{2}^{d}\bar{Q}_{L}^{0}\Phi_{2}d_{R}^{0}+Y_{1}^{\ell}\bar{L}_{L}^{0}\Phi_{1}\ell_{R}^{0}+Y_{2}^{\ell}\bar{L}_{L}^{0}\Phi_{2}\ell_{R}^{0}+h.c.
$$

with

$$
Q_{L}^{0}=\left(\begin{array}{c}
u_{L}\\
d_{L}
\end{array}\right),\;L^{0}=\left(\begin{array}{c}
\nu_{L}\\
e_{L}
\end{array}\right),\Phi_{1}=\left(\begin{array}{c}
\phi_{1}^{+}\\
\phi_{1}^{0}
\end{array}\right),\;\Phi_{2}=\left(\begin{array}{c}
\phi_{2}^{+}\\
\phi_{2}^{0}
\end{array}\right),\tilde{\Phi}_{j}=i\sigma_{2}\Phi_{j}^{*}.
$$

Here $$\Phi_i$$ $$(i=1, 2)$$ denotes the Higgs doublets and $$Y_i^f$$ stand for $$3\times3$$ Yukawa matrices. After SSB and algebraic manipulations, the Yukawa Lagrangian in term of physical states is given as follows:
