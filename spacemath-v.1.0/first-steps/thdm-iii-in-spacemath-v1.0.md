# THDM-III in SpaceMath v1.0

We will show how $$\texttt{SpaceMath v1.0}$$ works for the particular case of $$\mathcal{R}_{\tau}$$ ($$\texttt{Rtau}$$ in the $$\texttt{SpaceMath v1.0}$$ nomenclature).

1. Open a $$\texttt{Mathematica}$$ notebook,
2. Load $$\texttt{SpaceMath v1.0}$$ through $$\texttt{<<SpaceMath`}$$,
3. Define couplings as a function of the free model parameters. For the THDM-III case they are given in Table [#coupling-from-yukawa-lagrangian](thdm-iii-in-spacemath-v1.0.md#coupling-from-yukawa-lagrangian "mention").

{% tabs %}
{% tab title="Coupling from Yukawa Lagrangian" %}
$$\texttt{ghtt}=\frac{g}{2}\frac{m_t}{m_W}\left[\frac{\cos\alpha}{\sin\beta}\delta_{ij}-\frac{\sqrt{2}\cos(\alpha-\beta)}{g\sin\beta}\left(\frac{m_{W}}{m_{t}}\right)\left(\tilde{Y}_{2}^{U}\right)_{tt}\right]$$

$$\texttt{ghbb}=  						\frac{g}{2}\frac{m_{b}}{m_W}\left[-\frac{\sin\alpha}{\cos\beta}\delta_{ij}-\frac{\sqrt{2}\cos(\alpha-\beta)}{g\cos\beta}\left(\frac{m_{W}}{m_{b}}\right)\left(\tilde{Y}_{2}^{D}\right)_{bb}\right]$$

$$\texttt{gh}{\tau\tau}=  						\frac{g}{2}\frac{m_{{\tau}}}{m_W}\left[-\frac{\sin\alpha}{\cos\beta}\delta_{ij}-\frac{\sqrt{2}\cos(\alpha-\beta)}{g\cos\beta}\left(\frac{m_{W}}{m_{{\tau}}}\right)\left(\tilde{Y}_{2}^{\ell}\right)_{{\tau\tau}}\right]$$
{% endtab %}

{% tab title="Input to SpaceMath v1.0" %}
```wolfram
ghtt[a_,Att_,Cab_,tb_]:=(g/2)(mt/mW)((Cos[a]/tb*Cos[ArcTan[tb]])-(Sqrt[2]*Cab/(g*tb*Cos[ArcTan[tb]])*(mW/mt)*(mt/vev*Att)))	
```

```wolfram
ghbb[a_,Abb_,Cab_,tb_]:=(g/2)(mb/mW)((-Sin[a]*tb/Sin[ArcTan[tb]])+(Sqrt[2]*(Cab*tb)/(g*Sin[ArcTan[tb]])*(mW/mb)*(mb/vev*Abb)))
```

```wolfram
ghtautau[a_,Atata_,Cab_,tb_]:=(g/2)(mtau/mW)((-Sin[a]*tb/Sin[ArcTan[tb]])+(Sqrt[2]*(Cab*tb)/(g*Sin[ArcTan[tb]])*(mW/mtau)*(mtau/vev*Atata)))	
```
{% endtab %}
{% endtabs %}

We define $$\texttt{a}$$=$$\alpha$$, $$\texttt{Cab}$$=$$\cos(\alpha-\beta)$$, $$\texttt{sab}$$=$$\sin(\alpha-\beta)$$, $$\texttt{tb}$$=$$\tan\beta$$, $$\left(\tilde{Y}{2}^{F}\right){ij}=\sqrt{m_im_j}A_{ij}/\upsilon$$ and $$\sin\beta=\tan\beta\cos(\tan^{-1}(\tan\beta))$$. The terms $$\texttt{mf (f= fermions), mV (V=Z, W), g}$$ and $$\texttt{vev}$$ are the fermion masses, gauge boson masses, $$SU(2)$$ coupling constant and the vacuum expectation value, respectively. These quantities are loaded once $$\texttt{SpaceMath v1.0}$$ is executed. The file containing such information is $$\texttt{data.m}$$. From time to time the $$\texttt{data.m}$$ file is updated according to new information from the state of art, so that the user has available this new information simply to run the following instruction:

{% tabs %}
{% tab title="Data update " %}
```mathematica
UpdateSpaceMathData[]
```
{% endtab %}
{% endtabs %}
