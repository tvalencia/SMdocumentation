# THDM-III in SpaceMath v1.0

We will show how $$\texttt{SpaceMath v1.0}$$ works for the particular case of $$\mathcal{R}_{\tau}$$ ($$\texttt{Rtau}$$ in the $$\texttt{SpaceMath v1.0}$$ nomenclature).

1. Open a $$\texttt{Mathematica}$$ notebook,
2. Load $$\texttt{SpaceMath v1.0}$$ through $$\texttt{<<SpaceMath`}$$,
3. Define couplings as a function of the free model parameters. For the THDM-III case they are given in Table \ref{AcoplamientosTHDMIII}.

{% tabs %}
{% tab title="Coupling from Yukawa Lagrangian" %}

{% endtab %}

{% tab title="Input to SpaceMath v1.0" %}
..c$$\texttt{ghtt}=\frac{g}{2}\frac{m_t}{m_W}\left[\frac{\cos\alpha}{\sin\beta}\delta_{ij}-\frac{\sqrt{2}\cos(\alpha-\beta)}{g\sin\beta}\left(\frac{m_{W}}{m_{t}}\right)\left(\tilde{Y}_{2}^{U}\right)_{tt}\right]$$
{% endtab %}
{% endtabs %}

| Coupling from Yukawa Lagrangian                                                                                                                                                                                   | Input to SpaceMath v1.0                               |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------- |
| $$\texttt{ghtt}=\frac{g}{2}\frac{m_t}{m_W}\left[\frac{\cos\alpha}{\sin\beta}\delta_{ij}-\frac{\sqrt{2}\cos(\alpha-\beta)}{g\sin\beta}\left(\frac{m_{W}}{m_{t}}\right)\left(\tilde{Y}_{2}^{U}\right)_{tt}\right]$$ |                                                       |
|                                                                                                                                                                                                                   | $$\texttt{ghtt[a\_,Att\_,Cab\_,tb\_]:=(g/2)(mt/mW)}$$ |
|                                                                                                                                                                                                                   |                                                       |

