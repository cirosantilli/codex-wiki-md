<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an [action functional](../../../../action.md) $S[q]=\int_{t_i}^{t_f}L(q,\dot q,t)dt$, vary a path while fixing its endpoint coordinates. [Integration by parts](../../../../integration-by-parts.md) gives

$$
\delta S=\left[\sum_i\frac{\partial L}{\partial\dot q_i}\delta q_i\right]_{t_i}^{t_f}
+\int_{t_i}^{t_f}\sum_i\left[\frac{\partial L}{\partial q_i}-\frac d{dt}\frac{\partial L}{\partial\dot q_i}\right]\delta q_i\,dt.
$$

The endpoint term vanishes. Since the interior variations are arbitrary, stationarity gives

$$
\boxed{\frac d{dt}\frac{\partial L}{\partial\dot q_i}-\frac{\partial L}{\partial q_i}=0.}
$$

Define [canonical momentum](../../../../canonical-momentum.md) $p_i=\partial L/\partial\dot q_i$. For a regular [velocity](../../../../velocity.md) Hessian, these relations can be inverted for $\dot q(q,p,t)$, and the [Legendre transform](../../../../convex-conjugate.md) defines

$$
\boxed{H(q,p,t)=\sum_ip_i\dot q_i-L(q,\dot q,t).}
$$

Its differential is $dH=\sum_i(\dot q_i\,dp_i-L_{q_i}\,dq_i)-L_tdt$. Inserting the [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) already suggests the canonical equations.

To derive them directly from an [principle of stationary action](../../../../principle-of-stationary-action.md), vary the first-order [action](../../../../action.md) $I[q,p]=\int(\sum_ip_i\dot q_i-H)dt$ with independent $q,p$ and fixed endpoint $q$. Integrating $p_i\delta\dot q_i$ by parts gives

$$
\delta I=\int\sum_i\left[(\dot q_i-H_{p_i})\delta p_i+(-\dot p_i-H_{q_i})\delta q_i\right]dt.
$$

Therefore

$$
\boxed{\dot q_i=\frac{\partial H}{\partial p_i},\qquad
\dot p_i=-\frac{\partial H}{\partial q_i}.}
$$

The endpoint [momenta](../../../../momentum-split.md) need not be fixed. A singular [velocity](../../../../velocity.md) Hessian instead requires a constrained [Hamiltonian](../../../../hamiltonian.md) formulation; the ordinary Legendre inversion is an assumption, not an identity valid for every [Lagrangian](../../../../lagrangian.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the classical mechanics course of Part B of the physics course of the University of Oxford](../../../split.md)
5. [Classical mechanics course of Part B of the physics course of the University of Oxford](../../../../classical-mechanics-course-of-part-b-of-the-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
