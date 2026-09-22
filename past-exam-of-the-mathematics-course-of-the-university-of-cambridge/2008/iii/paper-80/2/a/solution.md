<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For fixed real $\kappa$, consider initial data $u_0\in L^2(0,1)$ and a solution continuous into $L^2$ at time zero, with homogeneous [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) for positive times. Existence, uniqueness and continuous dependence in this [norm](../../../../../../norm.md) give [Hadamard well-posedness](../../../../../../well-posed-problem.md).

To construct a solution, put $v(x,t)=e^{\kappa x}u(x,t)$. Substitution gives

$$
v_t=v_{xx}-\kappa^2v,\qquad v(0,t)=v(1,t)=0.
$$

Let $b_j=2\int_0^1e^{\kappa x}u_0(x)\sin(j\pi x)\,dx$. The [Fourier sine series](../../../../../../fourier-sine-series.md) solution is

$$
\boxed{u(x,t)=e^{-\kappa x}\sum_{j=1}^\infty b_j\sin(j\pi x)
 e^{-[(j\pi)^2+\kappa^2]t}.}
$$

Multiplication by $e^{\pm\kappa x}$ is bounded on $L^2(0,1)$. [Completeness](../../../../../../completeness.md) of the sine basis gives convergence to $u_0$ in $L^2$ at time zero, while the exponential decay gives smoothness for positive times and the required equation and boundary values. For a classical solution continuous up to the endpoints at time zero, the usual initial-boundary compatibility conditions are additionally required.

For the [energy method](../../../../../../energy-method.md), [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\begin{aligned}
\frac12\frac d{dt}\|u\|_{L^2}^2
&=\operatorname{Re}\int_0^1\overline u(u_{xx}+2\kappa u_x)\,dx\\
&=-\int_0^1|u_x|^2dx+\kappa[|u|^2]_0^1
=-\|u_x\|_{L^2}^2.
\end{aligned}
$$

Both boundary terms vanish. The same identity applies to the difference of two solutions, proving uniqueness and continuous dependence. The [Poincaré inequality](../../../../../../poincare-inequality.md) further gives

$$
\boxed{\|u(t)\|_{L^2}\leq e^{-\pi^2t}\|u_0\|_{L^2},}
$$

with the identical estimate for differences of initial data. This [Dirichlet convection-diffusion contraction](../../../../../../dirichlet-convection-diffusion-contraction.md) holds for **every real $\kappa$**, and its energy constant is independent of the drift strength.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
