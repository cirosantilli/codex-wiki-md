<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take real $\kappa$ and use the [L2 norm](../../../../../../l2-norm.md) on the spatial interval. Existence, uniqueness and continuous dependence are the three requirements of [Hadamard well-posedness](../../../../../../well-posed-problem.md). An [energy method](../../../../../../energy-method.md) supplies the decisive estimate. For a smooth solution with homogeneous [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md), [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\frac12\frac d{dt}\|u(t)\|_2^2
=\operatorname{Re}\int_0^1\overline u(u_{xx}+\kappa u_x)\,dx
=-\|u_x\|_2^2+\frac{\kappa}{2}[|u|^2]_0^1
=-\|u_x\|_2^2.
$$

The drift contributes only a boundary term, which vanishes. The [Poincaré inequality](../../../../../../poincare-inequality.md) $\|u_x\|_2^2\geq\pi^2\|u\|_2^2$ further gives

$$
\boxed{\|u(t)\|_2\leq e^{-\pi^2t}\|u(0)\|_2.}
$$

Apply the same argument to the difference of two solutions to obtain uniqueness and continuous dependence on the initial data.

For existence, use the [Dirichlet gauge transform for constant drift](../../../../../../dirichlet-gauge-transform-for-constant-drift.md): $w=e^{\kappa x/2}u$ satisfies $w_t=w_{xx}-\kappa^2w/4$ with zero boundary values. Expanding $w_0$ in its [Fourier sine series](../../../../../../fourier-sine-series.md) gives

$$
w(x,t)=\sum_{j=1}^{\infty}b_j
e^{-[(j\pi)^2+\kappa^2/4]t}\sin(j\pi x).
$$

For $u_0\in L^2(0,1)$ the series defines a solution continuous in $L^2$ down to $t=0$ and smooth for positive time; multiplication by the fixed bounded exponentials preserves this interpretation. Its energy estimate follows by approximation with smooth initial data. For a classical solution at the initial corners, require the usual smoothness and boundary compatibility instead. **The problem is well posed in $L^2$, with a contraction estimate independent of the initial data.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
