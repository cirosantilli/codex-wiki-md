<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Treat a small patch as the point [tensile-crack seismic source](../../../../../../tensile-crack-seismic-source.md) at $\mathbf y_0$, with $M(t)=K V(t)$ and $K=\lambda I+2\mu\mathbf n\mathbf n^{\mathsf T}$. Let $\mathbf e=(\mathbf x-\mathbf y_0)/R$, $\gamma=\mathbf e\cdot\mathbf n$, $\mathbf a=K\mathbf e$, $m=\mathbf e\cdot K\mathbf e$ and $s=\operatorname{tr}K$. Source convolution and an integration by parts give the [point-moment elastodynamic displacement](../../../../../../point-moment-elastodynamic-displacement.md)

$$
\boxed{u_i(\mathbf x,t)=\int M_{kj}(t')\,\partial_{y_j}G_{ik}(\mathbf x,\mathbf y_0,t-t')\,dt'
=-K_{kj}\partial_{x_j}(G_{ik}*V)}.
$$

The derivatives act on angular factors and on retarded times as well as on powers of $R$; keeping only the explicit $1/R$ Green-function terms would miss the static displacement.

Set $V_P=V(t-R/\alpha)$, $V_S=V(t-R/\beta)$ and

$$
I(R,t)=\int_{R/\alpha}^{R/\beta}\tau V(t-\tau)\,d\tau.
$$

Convolving the [elastodynamic Green tensor](../../../../../../elastodynamic-green-tensor.md) with the opening history gives

$$
4\pi\rho(G*V)_{ik}
=\frac{e_ie_k}{\alpha^2R}V_P
+\frac{\delta_{ik}-e_ie_k}{\beta^2R}V_S
+\frac{3e_ie_k-\delta_{ik}}{R^3}I.
$$

Use $\partial_jR=e_j$, $\partial_je_i=(\delta_{ij}-e_ie_j)/R$, $\partial_jV_P=-e_j\dot V_P/\alpha$, and

$$
\partial_R I=\frac R{\beta^2}V_S-\frac R{\alpha^2}V_P.
$$

For example, $K_{kj}\partial_j(e_ie_k/R)=[a_i+e_i(s-3m)]/R^2$, while differentiating the near-field angular tensor gives $[6a_i+3e_i s-15e_i m]/R^4$. Combining these with the endpoint terms in $\partial_R I$ yields

$$
\boxed{\begin{aligned}
4\pi\rho\mathbf u={}&\frac{\mathbf e m}{\alpha^3R}\dot V_P
+\frac{\mathbf a-\mathbf e m}{\beta^3R}\dot V_S\\
&+\frac{6\mathbf e m-2\mathbf a-\mathbf e s}{\alpha^2R^2}V_P
+\frac{3\mathbf a+\mathbf e s-6\mathbf e m}{\beta^2R^2}V_S\\
&+\frac{15\mathbf e m-6\mathbf a-3\mathbf e s}{R^4}I(R,t).
\end{aligned}}
$$

For the normal crack, $\mathbf a=\lambda\mathbf e+2\mu\gamma\mathbf n$, $m=\lambda+2\mu\gamma^2$, and $s=3\lambda+2\mu$. Explicitly, the three nonradiative vector coefficients in the last two lines are

$$
\begin{aligned}
\mathbf C_P&=(\lambda-2\mu+12\mu\gamma^2)\mathbf e-4\mu\gamma\mathbf n,\\
\mathbf C_S&=(2\mu-12\mu\gamma^2)\mathbf e+6\mu\gamma\mathbf n,\\
\mathbf C_I&=(30\mu\gamma^2-6\mu)\mathbf e-12\mu\gamma\mathbf n.
\end{aligned}
$$

Thus those lines are $\mathbf C_PV_P/(\alpha^2R^2)+\mathbf C_SV_S/(\beta^2R^2)+\mathbf C_I I/R^4$. The small-source approximation assumes the patch size is small relative to both $R$ and the wavelengths of interest; a finite crack is obtained by integrating the same point-patch expression over its surface with its local opening and normal.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
