<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Steady state.** In the [heat equation](../../../../heat-equation.md), time independence makes the second spatial [derivative](../../../../derivative.md) zero. The two endpoint [temperatures](../../../../temperature-split.md) therefore determine the linear profile

$$
\boxed{T_\infty(x)=T_0x/l.}
$$

Insulation is along the sides; the endpoint reservoirs can still exchange [heat](../../../../heat-split.md) with the rod.

**Transient solution.** Subtract the steady profile before applying [separation of variables](../../../../separation-of-variables.md): let $U=T-T_0x/l$. Then $U_t=\nu U_{xx}$, $U(0,t)=U(l,t)=0$ and $U(x,0)=-T_0x/l$ for $0<x<l$. Writing $U=X(x)\Theta(t)$ gives

$$
\frac{\Theta'}{\nu\Theta}=\frac{X''}{X}=-\mu,\qquad X''+\mu X=0,\qquad\Theta'+\nu\mu\Theta=0.
$$

The homogeneous [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md) exclude $\mu\leq0$ and select the [eigenfunctions](../../../../eigenfunction.md) $\sin(n\pi x/l)$ with [eigenvalues](../../../../eigenvalue.md) $\mu_n=(n\pi/l)^2$, $n\geq1$. Their [orthogonality](../../../../orthogonal-vectors.md) gives the [Fourier sine series](../../../../fourier-sine-series.md) coefficients

$$
b_n=\frac2l\int_0^l\left(-\frac{T_0x}l\right)\sin\frac{n\pi x}l\,dx=\frac{2T_0(-1)^n}{n\pi}.
$$

Here [integration by parts](../../../../integration-by-parts.md) uses $\int_0^l x\sin(n\pi x/l)\,dx=-l^2(-1)^n/(n\pi)$. Thus

$$
\boxed{T(x,t)=\frac{T_0x}l+\frac{2T_0}\pi\sum_{n=1}^\infty\frac{(-1)^n}{n}\sin\frac{n\pi x}l\,e^{-\nu n^2\pi^2t/l^2},\qquad t>0.}
$$

Every summand satisfies the [heat equation](../../../../heat-equation.md) and the homogeneous endpoint conditions, while the steady profile supplies the prescribed endpoint values. The initial [Fourier sine series](../../../../fourier-sine-series.md) equals $-T_0x/l$ in the open interval. At $(l,0)$ the initially cold rod and the suddenly imposed hot endpoint are incompatible; the formula describes the prescribed data for $t>0$ and the initial limit at interior points.

**Heat absorption.** Integrating in $x$ kills the even modes. With $a=\nu\pi^2/l^2$, the total [heat](../../../../heat-split.md) relative to the initial state is

$$
H(t)=\frac{\gamma T_0l}2-\frac{4\gamma T_0l}{\pi^2}\sum_{j=0}^\infty\frac{e^{-a(2j+1)^2t}}{(2j+1)^2}.
$$

Consequently the net rate of [heat](../../../../heat-split.md) absorption is

$$
\boxed{\frac{dH}{dt}=\frac{4\gamma\nu T_0}l\sum_{j=0}^\infty e^{-\nu\pi^2(2j+1)^2t/l^2}.}
$$

For each $t\geq\varepsilon>0$, any fixed number of differentiated modes is bounded by a polynomial in $n$ times $e^{-a\varepsilon n^2}$. These bounds have finite sums, proving [absolute convergence](../../../../absolute-convergence.md), [uniform convergence](../../../../uniform-convergence.md) on such time intervals and the validity of the integration and differentiation. In particular the displayed rate is finite for every $t>0$, positive when $T_0>0$, and tends to zero as equilibrium is approached. The same answer follows from the [heat equation](../../../../heat-equation.md) balance $H'=\gamma\nu[T_x(l,t)-T_x(0,t)]$; this subtracts loss at the cold endpoint from input at the hot endpoint.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
