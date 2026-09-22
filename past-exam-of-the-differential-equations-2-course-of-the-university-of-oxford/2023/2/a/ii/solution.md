<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use $t=x+1$. The [Legendre differential equation](../../../../../legendre-differential-equation.md) becomes

$$
t(2-t)y_{tt}+2(1-t)y_t+Ny=0.
$$

Substituting a [Frobenius series](../../../../../frobenius-solution.md) $y=t^r\sum_{k\geq0}a_kt^k$, $a_0\ne0$, gives the [indicial equation](../../../../../indicial-equation.md) $2r^2=0$: the [indicial root](../../../../../indicial-root.md) zero is repeated. For $r=0$, the coefficient of $t^k$ yields

$$
2(k+1)^2a_{k+1}+[n(n+1)-k(k+1)]a_k=0,
$$

or

$$
\boxed{a_{k+1}=\frac{(k-n)(k+n+1)}{2(k+1)^2}a_k}.
$$

For $0\leq k<n$ the multiplying factor is nonzero. At $k=n$ it vanishes, so $a_{n+1}$ and all later coefficients are zero. Thus one solution is a [polynomial](../../../../../polynomial-split.md) of exact [polynomial degree](../../../../../degree-of-a-polynomial.md) $n$, including a nonzero constant when $n=0$. Denote a chosen normalization by $P_n$.

The [linear recurrence relation](../../../../../linear-recurrence-relation.md) determines every analytic coefficient from $a_0$, so there cannot be a second independent analytic solution at $t=0$. To see the required logarithm explicitly, [reduction of order](../../../../../reduction-of-order.md) gives the second solution locally as

$$
P_n(x)\int^x\frac{ds}{(1-s^2)P_n(s)^2}.
$$

Near $t=0$, the integrand is $1/(2a_0^2t)$ plus an [analytic function](../../../../../holomorphic-function-split.md). After rescaling the second solution, its form is therefore

$$
\boxed{y_2(x)=P_n(x)\log(x+1)+\sum_{k=0}^\infty b_k(x+1)^k}.
$$

The analytic remainder converges locally; its constant term may be set to zero by adding a multiple of $P_n$. The nonzero logarithmic coefficient makes $y_2$ [linearly independent](../../../../../linear-independence.md) of $P_n$. This [Frobenius expansion of the Legendre equation at an endpoint](../../../../../frobenius-expansion-of-the-legendre-equation-at-an-endpoint.md) gives a [Logarithmic Frobenius solution](../../../../../logarithmic-solution-from-a-repeated-frobenius-exponent.md); the same endpoint calculation at $x=1$ explains why the independent [Legendre function of the second kind](../../../../../legendre-function-of-the-second-kind.md) is excluded when boundedness at both ends is required.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
