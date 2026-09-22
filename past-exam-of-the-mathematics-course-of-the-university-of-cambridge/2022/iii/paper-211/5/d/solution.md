<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Applying the [Itô product rule](../../../../../../ito-product-rule.md) to $YB$ makes its drift vanish automatically. For $YS$, the drift is

$$
YS(\mu-r-\lambda\sigma)\,dt.
$$

Thus both deflated prices are local martingales when

$$
\lambda=\frac{\mu-r}{\sigma}.
$$

Since self-financing gives $dX=\phi\,dB+\pi\,dS$, another application of the product rule, including $d[X,Y]$, cancels the drift and yields

$$
\boxed{d(X_tY_t)
=Y_t(\pi_tS_t\sigma-X_t\lambda)\,dW_t.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
