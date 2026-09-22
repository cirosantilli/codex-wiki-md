<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Localize to compact subintervals of $(0,\infty)$, so that the [Itô formula](../../../../../../ito-s-lemma.md) can be applied to $f(z)=\sqrt z$. Its derivatives are $f'(z)=1/(2\sqrt z)$ and $f''(z)=-1/(4z^{3/2})$, while $d[Z]_t=4Z_tdt$. Thus, before $\zeta$,

$$
\begin{aligned}
dR_t&=\frac1{2R_t}(2R_t\,dB_t+\gamma dt)
-\frac1{8R_t^3}(4R_t^2dt)\\
&=dB_t+\frac{\gamma-1}{2R_t}dt.
\end{aligned}
$$

Hence the [Bessel process](../../../../../../bessel-process.md) equation is

$$
\boxed{dR_t=dB_t+\frac{\gamma-1}{2R_t}dt,\qquad R_0=r,\quad t<\zeta.}
$$

The inverse-power drift is interpreted only while $R>0$; its boundary behaviour is justified next, not assumed in this calculation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
