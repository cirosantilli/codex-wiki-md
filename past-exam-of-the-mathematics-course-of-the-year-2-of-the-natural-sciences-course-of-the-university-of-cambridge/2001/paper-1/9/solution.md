<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

**Variational formulation.** Take real $p,q,w$ with $p,w>0$ in the interval, and impose homogeneous [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md), or other suitable conditions that cancel the boundary terms. The [functional](../../../../functional.md)

$$
J[y]=\int_a^b\left[p(x)(y')^2+q(x)y^2-\lambda w(x)y^2\right]dx
$$

has [Euler-Lagrange equation](../../../../euler-lagrange-equation.md)

$$
\frac d{dx}(2py')-2(q-\lambda w)y=0,
$$

which is equivalent to $-(py')'+qy-\lambda wy=0$. The same construction is constrained stationarity of the energy $\int[p(y')^2+qy^2]$ subject to $\int wy^2=1$, with $\lambda$ a [Lagrange multiplier](../../../../lagrange-multiplier.md). For fixed zero endpoint values, the variation vanishes at both ends; homogeneous zero-flux conditions also cancel the boundary term $[2py'\delta y]_a^b$.

Multiplying the differential equation by $y$ and using [integration by parts](../../../../integration-by-parts.md) gives the [Rayleigh quotient](../../../../rayleigh-quotient.md)

$$
\boxed{R[y]=\frac{\displaystyle\int_a^b[p(y')^2+qy^2]dx}{\displaystyle\int_a^bwy^2dx}.}
$$

For a nonzero admissible trial [function](../../../../function-split.md), $R[y]\geq\lambda_0$ by the [Rayleigh-Ritz variational principle](../../../../rayleigh-ritz-variational-principle.md). The [Rayleigh-Ritz method](../../../../rayleigh-ritz-method.md) chooses trial functions satisfying the endpoint conditions, often with adjustable coefficients, and minimizes this quotient over that trial family. Expanding $y=\sum c_ny_n$ in a normalized [eigenbasis](../../../../eigenbasis.md) shows why the lower bound holds: $R[y]=\sum\lambda_n c_n^2/\sum c_n^2$, a weighted average of [eigenvalues](../../../../eigenvalue.md) no smaller than the least one.

**Radial quadratic trial.** The radial problem becomes

$$
-(r^2\psi')'=\lambda r^2\psi,\qquad\psi(1)=0,\qquad\psi'(0)=0,
$$

where the printed endpoint notation $y$ refers to $\psi$. Thus $p=w=r^2$ and $q=0$. At the origin the vanishing $r^2$ and regularity of $\psi$ make the boundary term vanish; the weight must be retained in both numerator and denominator.

For a quadratic $\psi=A+Br+Cr^2$, the derivative condition sets $B=0$ and the outer condition gives $C=-A$. Overall amplitude cancels in the [Rayleigh quotient](../../../../rayleigh-quotient.md), so take $\widetilde\psi=1-r^2$. Then

$$
\int_0^1r^2(\widetilde\psi')^2dr=4\int_0^1r^4dr=\frac45,
$$

while

$$
\int_0^1r^2\widetilde\psi^2dr=\int_0^1(r^2-2r^4+r^6)dr=\frac13-\frac25+\frac17=\frac8{105}.
$$

Consequently

$$
\boxed{\widetilde\psi(r)=1-r^2,\qquad\widetilde\lambda_0=\frac{4/5}{8/105}=\frac{21}2=10.5.}
$$

**Why the estimate is higher.** For a regular radial [function](../../../../function-split.md) put $u=r\psi$. Then $u(0)=u(1)=0$, and direct differentiation transforms the equation to $u''+\lambda u=0$. Its first mode is $u=\sin(\pi r)$, corresponding to $\psi=\sin(\pi r)/r$ with its continuous value at the origin. Thus $\lambda_0=\pi^2$. The quadratic trial is not proportional to that [Spherical Bessel function](../../../../spherical-bessel-function.md), so it has nonzero components in higher modes. Its [Rayleigh quotient](../../../../rayleigh-quotient.md) is therefore strictly larger than $\pi^2$, in agreement with $21/2>\pi^2$.

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Paper 1](../../paper-1-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
