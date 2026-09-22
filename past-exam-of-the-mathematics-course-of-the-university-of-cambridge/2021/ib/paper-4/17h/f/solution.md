<h1 id="17h/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Set $\theta_0=1/2$ and $z=(\theta-1/2)^2$. Since

$$
\theta(1-\theta)=\frac14-z,
\qquad
0\leq z<\frac14,
$$

the risk is affine in $z$:

$$
g_{w,1/2}(\theta)
=\frac{w^2}{4n}
+z\left((1-w)^2-\frac{w^2}{n}\right).
$$

Its supremum is therefore controlled by the midpoint $z=0$ and the endpoint limit $z\to1/4$. Requiring both endpoint values to be at most the MLE's maximal risk $1/(4n)$ gives

$$
\frac{w^2}{4n}\leq\frac1{4n},
\qquad
\frac{(1-w)^2}{4}\leq\frac1{4n}.
$$

Equivalently,

$$
|w|\leq1,
\qquad
|1-w|\leq\frac1{\sqrt n}.
$$

Their intersection is

$$
\boxed{1-\frac1{\sqrt n}\leq w\leq1}.
$$

For precisely this range, the shrinkage estimator has maximal [mean squared error](../../../../../../mean-squared-error.md) no greater than that of $\widehat\theta$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [17H](../../17h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
