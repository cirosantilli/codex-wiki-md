<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The weaker plume detrains into the middle layer at $h_2$, while the stronger plume passes through it and feeds the upper layer at $h_1$. Middle-layer volume balance is

$$
Q_2(h_2)=Q_1(h_1)-Q_1(h_2).
$$

Using $Q_i(z)=C_QF_i^{1/3}z^{5/3}$ gives

$$
\boxed{
\frac{h_2}{h_1}
=\left[
1+\left(\frac{F_2}{F_1}\right)^{1/3}
\right]^{-3/5}
}.
$$

The middle layer receives buoyancy flux $F_2$ and loses volume $Q_2(h_2)$ by entrainment into the strong plume. The upper layer ultimately receives both source buoyancy fluxes and loses volume $Q_1(h_1)$ through the ceiling. Hence

$$
\boxed{
\widehat g'_{10}=\frac{F_2}{Q_2(h_2)},
\qquad
\widehat g'_{20}=\frac{F_1+F_2}{Q_1(h_1)}
}.
$$

The interior-minus-exterior pressure is constant below $h_2$, rises with slope $\rho_0\widehat g'_{10}$ in the middle layer, and with slope $\rho_0\widehat g'_{20}$ in the upper layer. Put

$$
\mathcal B
=\widehat g'_{10}(h_1-h_2)
+\widehat g'_{20}(H-h_1).
$$

Equal ideal openings split the total pressure difference equally, and the common ventilation rate is

$$
Q_1(h_1)=C_dA_f\sqrt{\mathcal B}
=C_dA_c\sqrt{\mathcal B}.
$$

Thus the required equal vent areas are

$$
\boxed{
A_f=A_c
=\frac{Q_1(h_1)}
{C_d\sqrt{
\widehat g'_{10}(h_1-h_2)
+\widehat g'_{20}(H-h_1)}}
}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
