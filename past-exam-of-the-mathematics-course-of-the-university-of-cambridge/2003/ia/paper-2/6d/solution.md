<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

For two solutions $y_1,y_2$, define the [Wronskian](../../../../../wronskian.md)

$$
W=y_1y_2'-y_1'y_2.
$$

Differentiate and substitute the [second-order linear differential equation](../../../../../second-order-linear-differential-equation.md):

$$
W'=y_1y_2''-y_1''y_2=-p(y_1y_2'-y_1'y_2)=-pW.
$$

Integration proves the [Abel identity](../../../../../abel-s-identity.md), including the identically zero case:

$$
\boxed{W(x)=W(x_0)\exp\left[-\int_{x_0}^xp(\xi)\,d\xi\right].}
$$

For $p=-2/x$, this is $W=Cx^2$ on either interval excluding zero, since the integral uses $\log|x|$. The coefficient singularity at zero must not be ignored.

Multiply the particular equation by $x^2$ and substitute the [Frobenius solution](../../../../../frobenius-solution.md) $y=x^\lambda\sum_{n\ge0}a_nx^n$. With $a_{-1}=a_{-2}=0$, equating coefficients gives

$$
\boxed{(n+\lambda)(n+\lambda-3)a_n=a_{n-2}.}
$$

The leading coefficient is nonzero, so the [indicial equation](../../../../../indicial-equation.md) is $\lambda(\lambda-3)=0$. Thus only $\lambda=0,3$ are possible, and the recurrences below construct both.

For $\lambda=0$, $a_1=0$, $a_2=-a_0/2$, and the $n=3$ recurrence reads $0=a_1=0$, leaving $a_3$ free. For all later indices,

$$
\boxed{a_{2k}=a_0\frac{1-2k}{(2k)!}\quad(k\ge0),\qquad
 a_{2k+3}=\frac{6a_3(k+1)}{(2k+3)!}\quad(k\ge0),\qquad a_1=0.}
$$

This is an [undetermined coefficient at Frobenius resonance](../../../../../undetermined-coefficient-at-frobenius-resonance.md); choosing $a_3=0$ selects a convenient even basis solution but is not forced by the differential equation.

For $\lambda=3$, all odd-indexed coefficients vanish and

$$
\boxed{a_{2k}=\frac{6a_0(k+1)}{(2k+3)!},\qquad a_{2k+1}=0\quad(k\ge0).}
$$

The factorial denominators show convergence for every finite $x$. Expanding the given [hyperbolic functions](../../../../../hyperbolic-function.md) directly yields

$$
\cosh x-x\sinh x=\sum_{k\ge0}\frac{1-2k}{(2k)!}x^{2k},
$$



$$
\sinh x-x\cosh x=-\sum_{k\ge0}\frac{2k+2}{(2k+3)!}x^{2k+3}.
$$

Consequently the exponent-zero family is $a_0(\cosh x-x\sinh x)-3a_3(\sinh x-x\cosh x)$, and the normalized exponent-three solution is $-3a_0(\sinh x-x\cosh x)$. This verifies the coefficient formulas and supplies two independent basis functions.

Finally $y_1'=-x\cosh x$ and $y_2'=-x\sinh x$, so

$$
W=(\cosh x-x\sinh x)(-x\sinh x)-(-x\cosh x)(\sinh x-x\cosh x)
=\boxed{-x^2}.
$$

This agrees with the Abel calculation. Its vanishing at zero does not contradict [independence](../../../../../independent-random-variables.md) on regular intervals: the original equation is singular there.

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
