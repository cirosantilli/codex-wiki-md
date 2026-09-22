<h1 id="11a/solution">Solution</h1>

↑ **Parent:** [11A](../11a.md)

At a [critical point](../../../../../critical-point.md) $p$ of a twice [continuously differentiable](../../../../../continuously-differentiable-function.md) real function, $\nabla f(p)=0$ and the [Taylor expansion](../../../../../taylor-expansion.md) is

$$
f(p+h)=f(p)+\tfrac12h^THh+o(|h|^2),
\qquad H=D^2f(p).
$$

The real symmetric [Hessian matrix](../../../../../hessian-matrix.md) has an [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md), so writing $h=\sum_i a_i u_i$ gives $h^THh=\sum_i\lambda_i a_i^2$. If every [eigenvalue](../../../../../eigenvalue.md) is positive, this quadratic form is at least $\lambda_{\min}|h|^2$, and the remainder cannot change its sign for sufficiently small nonzero $h$. Thus $p$ is a strict [local minimum](../../../../../local-minimum.md). If every [eigenvalue](../../../../../eigenvalue.md) is negative, the analogous argument gives a strict [local maximum](../../../../../local-maximum.md). If positive and negative [eigenvalues](../../../../../eigenvalue.md) both occur, displacement along the corresponding [eigenvectors](../../../../../eigenvector.md) gives values above and below $f(p)$, so $p$ is a [saddle point of a scalar function](../../../../../saddle-point-of-a-scalar-function.md).

The [second-derivative test](../../../../../second-derivative-test.md) can be inconclusive when the [Hessian matrix](../../../../../hessian-matrix.md) is singular and semidefinite: higher-order terms along directions in the [kernel of a linear map](../../../../../kernel-of-a-linear-map.md) matter. For example $x^2+y^4$ and $x^2-y^4$ have the same Hessian $\operatorname{diag}(2,0)$ at zero, but the first has a strict minimum and the second a [saddle point of a scalar function](../../../../../saddle-point-of-a-scalar-function.md). A zero [eigenvalue](../../../../../eigenvalue.md) does not prevent a saddle conclusion if other [eigenvalues](../../../../../eigenvalue.md) already have both signs.

For the given function write $r^2=x^2+y^2$. Its first [derivatives](../../../../../derivative.md) are

$$
f_x=y e^{-\alpha r^2}(1-2\alpha x^2),\qquad
f_y=x e^{-\alpha r^2}(1-2\alpha y^2).
$$

The origin is a [critical point](../../../../../critical-point.md) for every real $\alpha$, with

$$
D^2f(0,0)=\begin{pmatrix}0&1\\1&0\end{pmatrix}.
$$

Its [eigenvalues](../../../../../eigenvalue.md) are $1,-1$, so it is always a [saddle point of a scalar function](../../../../../saddle-point-of-a-scalar-function.md). If one coordinate at a [critical point](../../../../../critical-point.md) is zero, the other must also be zero. If both are nonzero, the [derivative](../../../../../derivative.md) equations force $x^2=y^2=1/(2\alpha)$, possible only for $\alpha>0$. Hence for $\alpha\leq0$ the origin is the only [critical point](../../../../../critical-point.md).

For $\alpha>0$ there are four additional [critical points](../../../../../critical-point.md),

$$
(x,y)=\frac1{\sqrt{2\alpha}}(\varepsilon,\eta),
\qquad \varepsilon,\eta\in\{-1,1\}.
$$

At such a point,

$$
f=\frac{\varepsilon\eta}{2\alpha e},\qquad
D^2f=-4\alpha xy\,e^{-1}I_2
=-\frac{2\varepsilon\eta}{e}I_2.
$$

Thus **the two equal-sign points are strict maxima, and the two opposite-sign points are strict minima**. They are global: $2|xy|\leq r^2$ implies

$$
|f(x,y)|\leq\frac{r^2}{2}e^{-\alpha r^2}
\leq\frac1{2\alpha e},
$$

where the last maximum occurs at $r^2=1/\alpha$ and equality also requires $x^2=y^2$.

As $\alpha\downarrow0$, the four nonzero [critical points](../../../../../critical-point.md) have distance $\alpha^{-1/2}$ from the origin and **escape to infinity**, rather than merging with the origin. Their values diverge as $\pm1/(2e\alpha)$. As $\alpha\uparrow0$ from below there are no extra [critical points](../../../../../critical-point.md), while the origin stays a saddle throughout. This is [critical points escaping to infinity in a Gaussian-weighted bilinear function](../../../../../critical-points-escaping-to-infinity-in-a-gaussian-weighted-bilinear-function.md).

## ↑ Ancestors (10)

1. [11A](../11a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
