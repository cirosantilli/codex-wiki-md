<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [Lasso](../../../../../lasso.md) minimizes

$$
\frac1{2n}\|Y-X\beta\|_2^2+\lambda\|\beta\|_1.
$$

Its [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) are

$$
\frac1nX^T(Y-X\widehat\beta)=\lambda\widehat z,
\qquad
\widehat z_j=
\begin{cases}
\operatorname{sgn}(\widehat\beta_j),&\widehat\beta_j\ne0,\\
\text{an element of }[-1,1],&\widehat\beta_j=0.
\end{cases}
$$

Since the columns of $X$ are centered, $X^T(\epsilon-\bar\epsilon\mathbf1)=X^T\epsilon$. Taking the inner product of the KKT equation with $\beta^0-\widehat\beta$ and using

$$
\widehat z^T\widehat\beta=\|\widehat\beta\|_1,
\qquad
\widehat z^T\beta^0\leq\|\beta^0\|_1
$$

gives

$$
\frac1n\|X(\beta^0-\widehat\beta)\|_2^2
\leq\frac1n|\epsilon^TX(\widehat\beta-\beta^0)|
+\lambda\|\beta^0\|_1-\lambda\|\widehat\beta\|_1.
$$

Put $\delta=\widehat\beta-\beta^0$. On $\Omega$,

$$
\frac1n|\epsilon^TX\delta|
\leq\frac\lambda2\|\delta\|_1.
$$

Using $\beta_N^0=0$ and

$$
\|\beta^0\|_1-\|\widehat\beta\|_1
\leq\|\delta_S\|_1-\|\delta_N\|_1
$$

in the basic inequality yields

$$
\frac1{n\lambda}\|X\delta\|_2^2
+\frac12\|\delta_N\|_1
<\frac32\|\delta_S\|_1.
$$

In particular $\delta$ lies in the [Lasso cone condition](../../../../../lasso-cone-condition.md).

The assumed [restricted eigenvalue condition](../../../../../restricted-eigenvalue-condition.md) and $\|\delta_S\|_1\leq\sqrt s\|\delta\|_2$ give

$$
\frac{\|X\delta\|_2^2}{n\lambda}
<\frac32\sqrt s\,\|\delta\|_2
\leq\frac{3\sqrt s}{2\kappa}
\frac{\|X\delta\|_2}{\sqrt n}.
$$

Canceling one prediction-norm factor and applying the restricted eigenvalue condition again gives

$$
\|\widehat\beta-\beta^0\|_2
<\frac{3\lambda\sqrt s}{2\kappa^2}.
$$

Choose

$$
\tau=\frac{3\lambda\sqrt s}{2\kappa^2}.
$$

Every null coordinate satisfies $|\widehat\beta_j|<\tau$. For $j\in S$,

$$
|\widehat\beta_j|
\geq|\beta_j^0|-\|\widehat\beta-\beta^0\|_\infty
>2\tau-\tau=\tau.
$$

**Thus $\widehat S^\tau=S$ on $\Omega$.**

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
