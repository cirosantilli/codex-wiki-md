<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Generate independent $U,V\sim\operatorname{Unif}(0,1)$ and use the [Box-Muller transform](../../../../../../box-muller-transform.md)

$$
\boxed{G_1=\sqrt{-2\log U}\cos(2\pi V),\qquad G_2=\sqrt{-2\log U}\sin(2\pi V).}
$$

For $R=\sqrt{-2\log U}$, $\mathbb P(R>r)=e^{-r^2/2}$, so its density is $re^{-r^2/2}$ on $r>0$. The angle $2\pi V$ is uniform on $[0,2\pi)$ and independent of $R$. Dividing the joint radial-angular density by the polar-coordinate Jacobian $r$ gives

$$
f_{G_1,G_2}(x,y)=\frac1{2\pi}e^{-(x^2+y^2)/2}
=\frac{e^{-x^2/2}}{\sqrt{2\pi}}\frac{e^{-y^2/2}}{\sqrt{2\pi}}.
$$

Thus **both outputs are independent and have the [standard normal distribution](../../../../../../standard-normal-distribution.md)**. Independent pairs of uniforms give further independent normal observations. The null event $U=0$ is excluded in implementation so the logarithm is finite.

## ↑ Ancestors (11)

1. [A](../a.md)
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
