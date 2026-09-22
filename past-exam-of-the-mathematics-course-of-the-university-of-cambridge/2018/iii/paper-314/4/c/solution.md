<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the Gaussian units of the paper, the total [magnetic pressure](../../../../../../magnetic-pressure.md) is $p_B=(B_R^2+B_\phi^2)/(8\pi)$. Define the initial [plasma beta](../../../../../../plasma-beta.md) $\beta_p=8\pi p_0/B_0^2\gg1$, assuming a nonzero initial field. The solution from part (b) gives

$$
p_B(R,t)=\frac{B_0^2}{8\pi}\left(\frac{R_0}{R}\right)^2\left[1+\frac94\frac{GMt^2}{R^3}\right],\qquad
\frac{p_B}{p}=\frac1{\beta_p}\left[1+\frac{9GMt^2}{4R^3}\right].
$$

For any $t>0$ this ratio decreases strictly with $R$, tends to infinity as $R\downarrow0$ and tends to $1/\beta_p<1$ as $R\to\infty$. The [magnetic-pressure equality radius under Keplerian winding](../../../../../../magnetic-pressure-equality-radius-under-keplerian-winding.md) is therefore unique in the formal profile on $R>0$:

$$
\boxed{R_{\rm eq}(t)=\left[\frac{9GM}{4(\beta_p-1)}\right]^{1/3}t^{2/3},\qquad\zeta=\frac23.}
$$

The same expression proves $p_B>p$ for $R<R_{\rm eq}$ and $p_B<p$ for $R>R_{\rm eq}$. At equality, $|B_\phi|/|B_R|=\sqrt{\beta_p-1}\gg1$, justifying the toroidal-dominated approximation

$$
R_{\rm eq}\simeq\left(\frac{9B_0^2GM}{32\pi p_0}\right)^{1/3}t^{2/3}.
$$

The source's existence claim refers to the indefinitely extended radial profile and the stated neglect of back-reaction. For a disk with a finite inner and outer edge, an equality radius lies in the disk only while the displayed value lies between those edges. If the initial field were zero, no magnetic winding or equality radius would occur.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
