<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume $h>0$. The functional is the third [forward difference](../../../../forward-difference.md): each [forward difference](../../../../forward-difference.md) lowers the [polynomial degree](../../../../degree-of-a-polynomial.md) by one, so it annihilates every [polynomial](../../../../polynomial-split.md) of degree at most two. Directly, $X[1]=-1+3-3+1=0$, $X[x]=3h-6h+3h=0$, and $X[x^2]=3h^2-12h^2+9h^2=0$.

The [Peano kernel theorem](../../../../peano-kernel-theorem.md) now gives $X[u]=\int_0^{3h}K(t)u^{(3)}(t)\,dt$, where the [Peano kernel of the third forward difference](../../../../peano-kernel-of-the-third-forward-difference.md) is

$$
K(t)=\frac12\left[3(h-t)_+^2-3(2h-t)_+^2+(3h-t)_+^2\right]
=\boxed{\begin{cases}
t^2/2,&0\leq t\leq h,\\
(-2t^2+6ht-3h^2)/2,&h\leq t\leq2h,\\
(3h-t)^2/2,&2h\leq t\leq3h.
\end{cases}}
$$

Here $s_+=\max(s,0)$ is the positive-part [truncated power function](../../../../truncated-power-function.md). The normalized [quadratic cardinal B-spline](../../../../quadratic-cardinal-b-spline.md) is

$$
B_2(s)=\frac12\left[s_+^2-3(s-1)_+^2+3(s-2)_+^2-(s-3)_+^2\right].
$$

Its three [polynomial](../../../../polynomial-split.md) pieces agree with the displayed kernel after rescaling, giving $\boxed{K(t)=h^2B_2(t/h)}$. Its knots are $0,h,2h,3h$ in the physical variable, and $K$ is positive throughout $(0,3h)$.

The kernel mass can be evaluated without integrating each piece: apply its representation to $u(x)=x^3/6$, whose third [derivative](../../../../derivative.md) is one. This gives $\int_0^{3h}K(t)\,dt=X[x^3/6]=h^3$. The [weighted mean value theorem for integrals](../../../../weighted-mean-value-theorem-for-integrals.md) with a nonnegative weight therefore yields

$$
\boxed{X[u]=h^3u^{(3)}(\xi),\qquad0<\xi<3h.}
$$

Continuity of $u^{(3)}$ and strict positivity of the weight in the interior place an attained weighted-average value in that open interval, including the constant-derivative case.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the approximation of functions course of the University of Oxford](../../../split.md)
5. [Approximation of functions course of the University of Oxford](../../../../approximation-of-functions-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
