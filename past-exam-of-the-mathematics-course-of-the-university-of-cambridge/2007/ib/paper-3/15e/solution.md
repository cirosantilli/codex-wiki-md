<h1 id="15e/solution">Solution</h1>

↑ **Parent:** [15E](../15e.md)

Seek a [power series](../../../../../power-series.md) $y(x)=\sum_{k\geq0}a_kx^k$ in the [Legendre differential equation](../../../../../legendre-differential-equation.md). Equating coefficients of $x^k$ gives

$$
(k+2)(k+1)a_{k+2}+\bigl(n(n+1)-k(k+1)\bigr)a_k=0,
$$

so

$$
\boxed{a_{k+2}=\frac{(k-n)(k+n+1)}{(k+2)(k+1)}a_k.}
$$

The even and odd coefficients form separate chains. Choose a nonzero seed of the same parity as $n$ and set the other seed to zero. In the chosen chain, none of the factors vanishes before $k=n$, and the factor $k-n$ vanishes at $k=n$. Therefore this chain terminates with a nonzero $a_n$: it gives a [polynomial](../../../../../polynomial-split.md) of degree exactly $n$.

To impose the normalization, its value at $x=1$ must be nonzero. Suppose a nonzero polynomial solution were $y=(x-1)^mq(x)$ with $m\geq1$ and $q(1)\ne0$. The lowest-order coefficient in $(1-x^2)y''-2xy'$ would be $-2m^2q(1)(x-1)^{m-1}$, whereas $n(n+1)y$ has order $m$. This cannot satisfy the equation. Thus divide by $y(1)$ to obtain the [Legendre polynomial](../../../../../legendre-polynomial.md) $P_n$ with $P_n(1)=1$. Substitution or the coefficient recurrence gives

$$
\boxed{P_0(x)=1,\qquad P_1(x)=x,\qquad P_2(x)=\frac12(3x^2-1).}
$$

For an axisymmetric solution of the [Laplace equation](../../../../../laplace-equation.md) regular at the two polar axes, the separated modes and their superposition in [spherical polar coordinates](../../../../../spherical-coordinate-system.md) are

$$
\phi_n(r,\theta)=\bigl(A_nr^n+B_nr^{-n-1}\bigr)P_n(\cos\theta),\qquad
\phi(r,\theta)=\sum_{n=0}^\infty\bigl(A_nr^n+B_nr^{-n-1}\bigr)P_n(\cos\theta).
$$

This is the usual [separation of variables](../../../../../separation-of-variables.md) expansion; the singular angular solutions are excluded by regularity at the axes.

Here $\sin^2\theta=\frac23(P_0(\cos\theta)-P_2(\cos\theta))$, so only degrees $0$ and $2$ are required. The degree-zero radial function $A_0+B_0/r$ takes the same value $2/3$ at $r=a,b$; since $a<b$, this forces $B_0=0$, $A_0=2/3$. Write the degree-two coefficient as $-(2/3)T(r)$, where $T=Ar^2+Br^{-3}$ and $T(a)=T(b)=1$. Multiplying these boundary equations by $a^3,b^3$ and subtracting gives

$$
A=\frac{b^3-a^3}{b^5-a^5},\qquad B=\frac{a^3b^3(b^2-a^2)}{b^5-a^5}.
$$

Consequently

$$
\boxed{\phi(r,\theta)=\frac23\left[1-\frac{(b^3-a^3)r^2+a^3b^3(b^2-a^2)r^{-3}}{b^5-a^5}P_2(\cos\theta)\right].}
$$

Each term is [harmonic](../../../../../harmonic-function.md) in the shell, and the radial factor is $1$ at both boundaries, so this satisfies both [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md). The [maximum principle for harmonic functions](../../../../../maximum-principle-for-harmonic-functions.md), applied to the difference of two solutions, proves uniqueness among solutions continuous on the closed shell.

## ↑ Ancestors (10)

1. [15E](../15e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
