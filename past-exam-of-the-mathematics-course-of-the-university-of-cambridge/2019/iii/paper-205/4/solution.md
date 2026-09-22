<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A vector $g$ is a [subgradient](../../../../../subgradient.md) of a [convex function](../../../../../convex-function.md) $f$ at $x$ when

$$
f(y)\geq f(x)+g^T(y-x)\qquad\text{for every }y.
$$

A point $x$ minimizes $f$ exactly when $0\in\partial f(x)$. For absolute value,

$$
\partial|x|=
\begin{cases}
\{-1\},&x<0,\\
[-1,1],&x=0,\\
\{1\},&x>0.
\end{cases}
$$

[Coordinate descent](../../../../../coordinate-descent.md) repeatedly minimizes the objective over one coordinate while holding the others fixed, cycling through coordinates until convergence.

The [Lasso](../../../../../lasso.md) solves

$$
\min_{\beta\in\mathbb R^p}
\frac1{2n}\|Y-X\beta\|_2^2+\lambda\|\beta\|_1.
$$

For the first update, define the partial residual and score

$$
r^{(0)}=Y-\sum_{j=2}^pX_j\widehat\beta_j^{(0)},
\qquad R=X_1^Tr^{(0)}.
$$

Since $\|X_1\|_2^2=n$, the coordinate objective differs by a constant from

$$
\frac12\beta_1^2-\frac Rn\beta_1+\lambda|\beta_1|.
$$

Its subgradient condition gives the [soft thresholding](../../../../../soft-thresholding.md) update

$$
\boxed{\widehat\beta_1^{(1)}=S_\lambda(R/n).}
$$

For the stated [Berhu penalty](../../../../../berhu-penalty.md), the derivative is $\operatorname{sgn}(t)$ when $0<|t|\leq\delta$ and $t/\delta$ when $|t|>\delta$. The coordinatewise [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) therefore give

$$
\boxed{
\widehat\beta_1^{(1)}=
\begin{cases}
S_\lambda(R/n),&|S_\lambda(R/n)|\leq\delta,\\[2mm]
\dfrac{R/n}{1+\lambda/\delta},&\text{otherwise}.
\end{cases}}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
