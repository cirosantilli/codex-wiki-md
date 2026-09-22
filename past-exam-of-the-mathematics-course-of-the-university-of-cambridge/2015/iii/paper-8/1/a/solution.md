<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $z=(x,v)$ and let $\Phi(t,s,z)$ denote the [Hamiltonian flow](../../../../../../hamiltonian-flow.md) from time $s$ to time $t$. The [characteristic curves](../../../../../../characteristic-curve.md) satisfy [Hamilton's equations](../../../../../../hamilton-s-equations.md):

$$
\boxed{\dot X_i(t)=\partial_{v_i}H(t,X(t),V(t)),\qquad
\dot V_i(t)=-\partial_{x_i}H(t,X(t),V(t)),\qquad
(X(s),V(s))=(x,v).}
$$

The [Hamiltonian Liouville equation](../../../../../../hamiltonian-liouville-equation.md) then reduces along each curve to

$$
\frac d{dt}f(t,X(t),V(t))=h(t,X(t),V(t)).
$$

The signs and derivative variables here are those in the PDF.

The [global characteristic flow for a Hamiltonian with bounded Hessian](../../../../../../global-characteristic-flow-for-a-hamiltonian-with-bounded-hessian.md) follows, for example, from $H\in C^2(\mathbb R\times\mathbb R^{2d})$ and, for every finite $T$,

$$
\sup_{|t|\leq T,\ z\in\mathbb R^{2d}}\|D_z^2H(t,z)\|\leq L_T<\infty,\qquad
\sup_{|t|\leq T}|\nabla_zH(t,0)|\leq A_T<\infty.
$$

Thus the [Hamiltonian vector field](../../../../../../hamiltonian-vector-field.md) $b=(\nabla_vH,-\nabla_xH)$ is globally [Lipschitz continuous](../../../../../../lipschitz-continuity.md) in $z$ on each finite time interval and satisfies $|b(t,z)|\leq A_T+L_T|z|$. The [Picard-Lindelöf theorem](../../../../../../picard-lindelof-theorem.md) gives local existence and uniqueness, while the [Gronwall inequality](../../../../../../gronwall-inequality.md) gives, for example,

$$
|\Phi(t,s,z)|\leq (|z|+A_T|t-s|)e^{L_T|t-s|}
\qquad(|s|,|t|\leq T).
$$

This excludes finite-time escape. **There is a unique [Hamiltonian flow](../../../../../../hamiltonian-flow.md) for all finite forward and backward times**, and $\Phi(s,t)$ is the inverse of $\Phi(t,s)$. These sufficient conditions are deliberately stronger than necessary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
