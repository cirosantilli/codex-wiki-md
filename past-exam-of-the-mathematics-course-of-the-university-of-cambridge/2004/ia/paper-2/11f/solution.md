<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

Take $\lambda>0$ as the rate of the [exponential distribution](../../../../../exponential-distribution.md). By [independence](../../../../../independent-random-variables.md), the [joint probability density](../../../../../joint-probability-density.md) of the original pair is $\lambda^2e^{-\lambda(x_1+x_2)}$ on $x_1,x_2>0$. Put $s=Y_1$, $r=Y_2$. The inverse [change of variables](../../../../../change-of-variables-formula.md) is

$$
x_1=\frac{sr}{1+r},\qquad x_2=\frac{s}{1+r},\qquad s>0,\ r>0.
$$

Its [Jacobian determinant](../../../../../jacobian-determinant.md) is

$$
\det\frac{\partial(x_1,x_2)}{\partial(s,r)}
=\det\begin{pmatrix}r/(1+r)&s/(1+r)^2\\1/(1+r)&-s/(1+r)^2\end{pmatrix}
=-\frac{s}{(1+r)^2}.
$$

Using the absolute value in the [change of variables formula](../../../../../change-of-variables-formula.md), the transformed [joint probability density](../../../../../joint-probability-density.md) is

$$
\boxed{f_{Y_1,Y_2}(s,r)=\frac{\lambda^2s e^{-\lambda s}}{(1+r)^2}\quad(s>0,r>0),}
$$

and zero otherwise. The support is the entire positive quadrant, and the factors are separately normalized:

$$
\int_0^\infty\lambda^2s e^{-\lambda s}\,ds=1,
\qquad \int_0^\infty\frac{dr}{(1+r)^2}=1.
$$

Integrating out either variable therefore yields these factors as the [marginal densities](../../../../../marginal-density.md). Factorization of the [joint probability density](../../../../../joint-probability-density.md) proves [independence](../../../../../independent-random-variables.md), with

$$
\boxed{f_{Y_1}(s)=\lambda^2s e^{-\lambda s}\ (s>0),\qquad f_{Y_2}(r)=\frac1{(1+r)^2}\ (r>0).}
$$

The sum has a shape-two [gamma distribution](../../../../../gamma-distribution.md), and the ratio has a [beta-prime distribution](../../../../../beta-prime-distribution.md) with parameters one and one, independent of $\lambda$. Its [cumulative distribution function](../../../../../cumulative-distribution-function.md) is $r/(1+r)$ for $r>0$.

## ↑ Ancestors (11)

1. [11F](../11f.md)
2. [Section II](../section-ii.md)
3. [Paper 2](../../paper-2-split.md)
4. [Ia](../../split.md)
5. [2004](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
