<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume the denominators are defined, so $c,d\ne0$. For a [descent direction](../../../../descent-direction.md) $p$, set $\varphi(\alpha)=f(x+\alpha p)$. The [Wolfe conditions](../../../../wolfe-conditions.md) are

$$
\varphi(\alpha)\leq\varphi(0)+\sigma\alpha\varphi'(0),\qquad
\varphi'(\alpha)\geq\eta\varphi'(0),\qquad0<\sigma<\eta<1.
$$

The first is sufficient decrease and the second is the curvature condition. Here

$$
H=\nabla^2 f=
\begin{pmatrix}c^{-2}+d^{-2}&c^{-2}-d^{-2}\\c^{-2}-d^{-2}&c^{-2}+d^{-2}\end{pmatrix}
$$

is positive definite, with [eigenvalues](../../../../eigenvalue.md) $2/c^2,2/d^2$. The exact step is

$$
\alpha_*=-\frac{\nabla f(x)^Tp}{p^THp}>0.
$$

It gives $\varphi'(\alpha_*)=0$, so the curvature condition holds. Its decrease is $\varphi(\alpha_*)-\varphi(0)=\alpha_*\varphi'(0)/2$, so sufficient decrease holds for the usual choice $0<\sigma\leq1/2$, $\sigma<\eta<1$. Hence **exact searches satisfy Wolfe with an Armijo constant at most one half**. If one allowed $\sigma>1/2$, even an exact quadratic minimizer would fail that condition; the parameter range matters.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
