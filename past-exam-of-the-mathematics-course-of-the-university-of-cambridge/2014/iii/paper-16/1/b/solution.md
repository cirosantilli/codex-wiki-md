<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The passage to [Hamiltonian mechanics](../../../../../../hamiltonian-mechanics.md) uses the [Legendre transform in mechanics](../../../../../../legendre-transform-in-mechanics.md). Assume a [regular Lagrangian](../../../../../../regular-lagrangian.md): the velocity [Hessian matrix](../../../../../../hessian-matrix.md) $(\partial^2L/\partial v^i\partial v^j)$ is invertible. Then

$$
p_i=\frac{\partial L}{\partial v^i}
$$

defines a locally invertible map from the [tangent bundle](../../../../../../tangent-bundle.md) to the [cotangent bundle](../../../../../../cotangent-bundle.md). Write its local inverse as $v=v(t,q,p)$ and define the [Hamiltonian](../../../../../../hamiltonian.md)

$$
H(t,q,p)=p_iv^i-L(t,q,v).
$$

Differentiating this expression, all terms containing $dv$ cancel because $p_i=L_{v^i}$. Hence

$$
dH=v^i\,dp_i-L_{q^i}\,dq^i-L_t\,dt,
\qquad H_{p_i}=v^i,\quad H_{q^i}=-L_{q^i}.
$$

The [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md) become [Hamilton's equations](../../../../../../hamilton-s-equations.md):

$$
\boxed{\dot q^i=H_{p_i},\qquad\dot p_i=-H_{q^i}.}
$$

Conversely, a solution of [Hamilton's equations](../../../../../../hamilton-s-equations.md) satisfies $\dot q=v(t,q,p)$, hence $p=L_v(t,q,\dot q)$, and $\dot p=L_q$ recovers the [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md). This proves local equivalence of the two descriptions.

On the [cotangent bundle](../../../../../../cotangent-bundle.md), choose the canonical [symplectic form](../../../../../../symplectic-form.md) $\omega_{\mathrm{can}}=\sum_i dq^i\wedge dp_i=-d\lambda$ and the convention $\iota_{X_H}\omega_{\mathrm{can}}=dH$. Then $X_H=\sum_i(H_{p_i}\partial_{q^i}-H_{q^i}\partial_{p_i})$, so its integral curves are exactly the phase-space equations above. **This sign convention is used throughout these solutions.** For a [hyperregular Lagrangian](../../../../../../hyperregular-lagrangian.md), the [Legendre transform in mechanics](../../../../../../legendre-transform-in-mechanics.md) is globally invertible and gives global equivalence; regularity alone only gives local equivalence. A singular velocity [Hessian matrix](../../../../../../hessian-matrix.md) may instead produce constraints, so the ordinary unconstrained argument does not apply to every [Lagrangian](../../../../../../lagrangian.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
