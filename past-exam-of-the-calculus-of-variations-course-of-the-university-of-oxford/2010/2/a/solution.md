<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a fixed-endpoint variation $\varphi\in W^{1,\infty}_0(a,b)$, the [second variation](../../../../second-variation.md) is

$$
\delta^2I(\bar u)(\varphi,\varphi)=\left.\frac{d^2}{dt^2}I(\bar u+t\varphi)\right|_{t=0}=\int_a^b\left(f_{vv}\varphi'^2+2f_{uv}\varphi\varphi'+f_{uu}\varphi^2\right)dx,
$$

where all coefficients are evaluated at $(x,\bar u(x),\bar u'(x))$. The notation $\delta^2I(\bar u)>0$ means this is strictly positive for every nonzero admissible variation. This is [pointwise](../../../../pointwise-convergence.md) positive definiteness of the [quadratic form](../../../../quadratic-form-split.md), not an assertion of a prescribed uniform lower bound.

Put

$$
P=f_{vv},\qquad Q=f_{uu}-\frac d{dx}f_{uv}.
$$

After [integration by parts](../../../../integration-by-parts.md), the form is $q(\varphi)=\int_a^b(P\varphi'^2+Q\varphi^2)\,dx$. Its [Jacobi equation](../../../../jacobi-equation.md) is

$$
\boxed{-(Pw')'+Qw=0.}
$$

In the regular case $P>0$ on $[a,b]$, a [conjugate point](../../../../conjugate-point.md) $c\in(a,b]$ to $a$ is a point for which a nonzero solution satisfies $w(a)=w(c)=0$. Equivalently it is a zero of the normalized solution with $w(a)=0$, $P(a)w'(a)=1$.

Under this regular [Strengthened Legendre condition](../../../../strengthened-legendre-condition.md), the [Jacobi positivity criterion](../../../../jacobi-positivity-criterion.md) is

$$
\boxed{q>0\iff\text{there is no conjugate point to }a\text{ in }(a,b].}
$$

The endpoint $b$ must be excluded as a [conjugate point](../../../../conjugate-point.md) too. To prove necessity, suppose a Jacobi solution vanishes at $a$ and $c$. Define $\varphi=w$ on $[a,c]$ and zero on $[c,b]$. It is a nonzero [Lipschitz](../../../../lipschitz-continuity.md) admissible variation, and

$$
q(\varphi)=\int_a^c(Pw'^2+Qw^2)dx=[Pww']_a^c=0,
$$

a contradiction. For completeness, the converse follows from the [Jacobi identity for the second variation](../../../../jacobi-identity-for-the-second-variation.md): when the normalized $w$ has no further zero,

$$
q(\varphi)=\int_a^bP\left(\varphi'-\frac{w'}w\varphi\right)^2dx.
$$

The boundary contribution $[P(w'/w)\varphi^2]_a^b$ vanishes, including the limit at $a$ since $w$ has a simple zero and $\varphi=O(x-a)$. Equality forces $\varphi=Cw$, and $\varphi(b)=0$ with $w(b)\ne0$ forces $C=0$.

Independently of regularity, positivity necessarily implies the ordinary [Legendre necessary condition](../../../../legendre-necessary-condition.md) $P\geq0$. If $P<0$ on an interval, localized rapidly oscillating test functions have a negative [derivative](../../../../derivative.md) contribution of order frequency squared, dominating the bounded zero-order term. This contradicts positivity.

The assumptions stated here do not themselves impose $P>0$. That strengthened condition is a regularity hypothesis for the familiar Jacobi criterion, and is not necessary for strict positivity: the integrand $f=u^2$ gives $q(\varphi)=2\int\varphi^2>0$ with $P=0$. For a criterion covering the full possibly degenerate class, use [Regularized Jacobi criterion for a degenerate second variation](../../../../regularized-jacobi-criterion-for-a-degenerate-second-variation.md). The following conditions are necessary and sufficient:

- $P\geq0$;
- for every $\eta>0$, the regular equation $-((P+\eta)w')'+Qw=0$ has no [conjugate point](../../../../conjugate-point.md) to $a$ in $(a,b]$;
- the original weak Jacobi boundary problem has no nonzero [Lipschitz](../../../../lipschitz-continuity.md) solution with zero endpoint values.

These conditions are necessary because $q>0$ gives $q_\eta(\varphi)=q(\varphi)+\eta\int\varphi'^2>0$, so the regular criterion just proved applies; a weak Jacobi solution tested against itself would give $q=0$. They are sufficient as well: the regular criterion gives $q_\eta>0$ for every $\eta>0$, hence $q\geq0$ by letting $\eta\downarrow0$. If $q(\varphi)=0$, nonnegativity of $q(\varphi+t\psi)$ for every real $t$ forces its mixed bilinear term to vanish for every test $\psi$. This is precisely the weak [Jacobi equation](../../../../jacobi-equation.md). The third condition then forces $\varphi=0$. Thus the criterion treats degeneracy without silently assuming the strengthened condition.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the calculus of variations course of the University of Oxford](../../../split.md)
5. [Calculus of variations course of the University of Oxford](../../../../calculus-of-variations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
