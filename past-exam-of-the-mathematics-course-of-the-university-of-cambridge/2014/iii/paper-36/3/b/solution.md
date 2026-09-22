<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For fixed parameters $(a,b)$, every new error is independent of the previous observations. Put $\varphi_0(z)=(2\pi)^{-1/2}e^{-z^2/2}$. Since $X_0=X_1=0$, the first three conditional densities are

$$
\boxed{f_{X_2\mid X_1}(x_2\mid0)=\varphi_0(x_2),\qquad
f_{X_3\mid X_2,X_1}(x_3\mid x_2,0)=\varphi_0(x_3-ax_2),}
$$

and

$$
\boxed{f_{X_4\mid X_3,X_2,X_1}(x_4\mid x_3,x_2,0)=\varphi_0(x_4-ax_3-bx_2).}
$$

In general,

$$
\boxed{X_{t+2}\mid(X_{t+1},\ldots,X_1),a,b\sim N(aX_{t+1}+bX_t,1).}
$$

Its density is $\varphi_0(x_{t+2}-ax_{t+1}-bx_t)$. The recursion is interpreted from $t=0$, as required to define $X_2$ from the two given initial values. These are parameter-conditional sampling distributions; integrating over the prior would instead give predictive mixtures.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
