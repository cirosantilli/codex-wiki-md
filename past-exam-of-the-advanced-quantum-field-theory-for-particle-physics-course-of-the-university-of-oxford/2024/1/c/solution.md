<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An [operator equation in a path integral](../../../../operator-equation-in-a-path-integral.md) $\mathcal O(x)=0$ means that insertion of $\mathcal O(x)$ into every [time-ordered correlation function](../../../../time-ordered-correlation-function.md) vanishes when $x$ is separated from the other insertion points. At coincident points, [Ward identity contact terms](../../../../ward-identity-contact-terms.md) can remain; an [operator equation](../../../../operator-equation-in-a-path-integral.md) does not assert that these distributions vanish.

Let $X$ be a product of local insertions. Make the local phase change of integration variables from part [b](../b.md). The [functional measure](../../../../functional-measure.md) has unit [functional Jacobian](../../../../functional-jacobian.md): the opposite phases of $\psi$ and $\bar\psi$ cancel in a vector-symmetry-preserving [regularization in quantum field theory](../../../../regularization-in-quantum-field-theory.md). There is no vector [gauge anomaly](../../../../gauge-anomaly.md). Invariance under a change of integration variables gives

$$
0=\langle\delta_\alpha X\rangle
+i\int d^4x\,\alpha(x)\langle T\{\partial_\mu j^\mu(x)X\}\rangle.
$$

If $X=\prod_r\mathcal O_r(x_r)$ and $\delta_\alpha\mathcal O_r=iq_r\alpha(x_r)\mathcal O_r$, comparison of the coefficients of the arbitrary $\alpha(x)$ yields the [Ward-Takahashi identity](../../../../ward-identity.md)

$$
\boxed{\langle T\{\partial_\mu j^\mu(x)X\}\rangle
=-\sum_rq_r\delta^{(4)}(x-x_r)\langle TX\rangle.}
$$

Consequently $\partial_\mu j^\mu=0$ is an [operator equation](../../../../operator-equation-in-a-path-integral.md) at separated points. This is stronger than just $\langle\partial_\mu j^\mu\rangle=0$. For example, $X=\psi(y)\bar\psi(z)$ has $q_y=1$, $q_z=-1$, so its two [Ward identity contact terms](../../../../ward-identity-contact-terms.md) are $[-\delta^{(4)}(x-y)+\delta^{(4)}(x-z)]\langle T\psi(y)\bar\psi(z)\rangle$; dropping them would give a false identity. Equivalently, the [Dirac equation](../../../../dirac-equation.md) and the [adjoint Dirac equation](../../../../adjoint-dirac-equation.md) give $\partial_\mu(\bar\psi\gamma^\mu\psi)=0$, with the same coincident-point qualification in [time-ordered correlation functions](../../../../time-ordered-correlation-function.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
