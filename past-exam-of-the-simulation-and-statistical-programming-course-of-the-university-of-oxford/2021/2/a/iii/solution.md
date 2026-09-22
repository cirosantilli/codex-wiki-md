<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $t=1-\rho\in(0,1)$. The target [Poisson distribution](../../../../../poisson-distribution.md) and proposal [geometric distribution](../../../../../geometric-distribution.md) have [probability mass functions](../../../../../probability-mass-function.md) $p_k=e^{-\lambda}\lambda^k/k!$ and $q_k=(1-t)t^k$. Their ratio is

$$
R_k(t)=\frac{p_k}{q_k}=\frac{e^{-\lambda}}{1-t}\frac{(\lambda/t)^k}{k!}.
$$

The successive ratio $R_{k+1}/R_k=\lambda/[t(k+1)]$ shows that a maximizing integer is $m=\lfloor\lambda/t\rfloor$, with a tie at $m-1$ when $\lambda/t$ is an integer. Thus the tight envelope is

$$
\boxed{M(t)=\frac{e^{-\lambda}}{1-t}\frac{(\lambda/t)^m}{m!},\qquad m=\lfloor\lambda/t\rfloor.}
$$

For any fixed $t$, draw $Y\sim\operatorname{Geom}(1-t)$ using (ii)'s inversion formula with this new parameter, and draw an [independent](../../../../../independent-random-variables.md) $U$ from the [uniform distribution](../../../../../continuous-uniform-distribution.md) on $(0,1)$. Accept when

$$
\boxed{U\leq\frac{R_Y(t)}{M(t)}=\frac{m!}{Y!}\left(\frac{\lambda}{t}\right)^{Y-m};}
$$

otherwise restart. The acceptance [probability](../../../../../probability.md) is $1/M(t)$ and the expected number of proposals is $M(t)$.

To minimize that expected count, set $K=\lceil\lambda\rceil$. The exact answer is

$$
\boxed{t_* =\min\!\left\{\frac{\lambda}{K},\frac{K}{K+1}\right\},\qquad
\rho_*=1-t_*=\max\!\left\{1-\frac{\lambda}{K},\frac1{K+1}\right\}.}
$$

Here is a proof that includes the changes of maximizing integer. Each $\log R_k(t)$ is a [convex function](../../../../../convex-function.md) of $t$, since its second [derivative](../../../../../derivative.md) is $(1-t)^{-2}+k/t^2>0$. Their pointwise maximum $\log M(t)$ is also a [convex function](../../../../../convex-function.md). When $m$ is fixed its [derivative](../../../../../derivative.md) is

$$
\frac{d}{dt}\log M(t)=\frac1{1-t}-\frac mt.
$$

If $K-1<\lambda\leq K^2/(K+1)$, take $t_* =\lambda/K$, where $m$ changes from $K$ on the left to $K-1$ on the right. The left [derivative](../../../../../derivative.md) is nonpositive because $\lambda\leq K^2/(K+1)$; the right [derivative](../../../../../derivative.md) is nonnegative because $\lambda\geq K-1$. This is a minimum. If $K^2/(K+1)<\lambda\leq K$, take $t_*=K/(K+1)$. There $K<\lambda/t_*\leq K+1$ and the active branch has $m=K$ except for the endpoint tie; its [derivative](../../../../../derivative.md) vanishes. Convexity again proves the global minimum. The formulas agree at the boundary.

For a fully specified optimal algorithm, compute $K,t_*,\rho_*$ and $m_*=\lfloor\lambda/t_*\rfloor$ once, then use the preceding acceptance test with $t=t_*$ and $m=m_*$. At an integer tie either maximizing integer gives the same test. In code, factorials can be evaluated through the [logarithm](../../../../../logarithm.md) of the [gamma function](../../../../../gamma-function.md):

$$
\log a_Y=\log\Gamma(m_*+1)-\log\Gamma(Y+1)+(Y-m_*)\log(\lambda/t_*),
$$

and acceptance is $\log U\leq\min(0,\log a_Y)$. This avoids overflowing factorials.

The optimum minimizes expected trials, the usual idealization of time when each proposal and test has constant cost. Actual runtime also depends on the implementation of discrete inversion and factorial evaluation. Simply minimizing an upper bound for $M(t)$ would not necessarily give the exact optimum above; see [optimal geometric envelope for a Poisson distribution](../../../../../optimal-geometric-envelope-for-a-poisson-distribution.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
