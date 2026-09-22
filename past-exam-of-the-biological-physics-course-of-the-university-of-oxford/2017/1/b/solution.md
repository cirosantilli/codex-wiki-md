<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [strong Hill autorepression response](../../../../strong-hill-autorepression-response.md), in the requested approximation, $\dot Y=\beta K^nY^{-n}-\alpha Y$. Put $z=Y^{n+1}$. Then

$$
\dot z=(n+1)(\beta K^n-\alpha z),\qquad
z(t)=\frac{\beta K^n}{\alpha}[1-e^{-(n+1)\alpha t}],
$$

so the formal zero-initial-concentration solution is

$$
\boxed{Y(t)=\left(\frac{\beta K^n}{\alpha}\right)^{1/(n+1)}
[1-e^{-(n+1)\alpha t}]^{1/(n+1)},\qquad
Y_{\rm st}=\left(\frac{\beta K^n}{\alpha}\right)^{1/(n+1)}.}
$$

Setting $Y(T_{1/2})=Y_{\rm st}/2$ gives

$$
\boxed{T_{1/2}=\frac{-\log(1-2^{-(n+1)})}{(n+1)\alpha},\qquad
\frac{T_{1/2}}{T_{1/2}^{(0)}}=
\frac{-\log(1-2^{-(n+1)})}{(n+1)\log2}.}
$$

The formal ratio decreases with positive $n$; for $n=1$ it is about $0.208$, and for $n=2$ about $0.0642$. Its large-$n$ asymptote is $2^{-(n+1)}/[(n+1)\log2]$. This is a [nonlinear](../../../../nonlinear-ordinary-differential-equation.md) half-response time, not simply the near-equilibrium [relaxation time](../../../../time-constant.md) $1/[(n+1)\alpha]$.

**Approximation qualification.** The omitted initial layer is precisely the one the source permits us to ignore: the approximate derivative diverges at $Y=0$, whereas the full [Hill equation](../../../../hill-equation.md) has initial slope $\beta$. The approximation is not uniform as $n\to\infty$ at fixed $R=\beta/(\alpha K)$. Strong repression already at half of the final [concentration](../../../../concentration.md) needs $R^{1/(n+1)}/2\gg1$. The actual [Hill equation](../../../../hill-equation.md) obeys $\dot Y\le\beta$, so $T_{1/2}\ge Y_{\rm st}/(2\beta)$. Its steep-switch limit approaches the logic-response scale in [a](../a.md); the formal vanishing large-$n$ result above cannot be extrapolated past its regime of validity.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
