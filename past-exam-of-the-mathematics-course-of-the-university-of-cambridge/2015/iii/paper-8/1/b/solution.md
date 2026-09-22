<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $S_t(z)=\Phi(t,0,z)$, differentiability with respect to initial data gives the variational equation

$$
Y'(t)=D_zb(t,S_t(z))Y(t),\qquad Y(0)=I_{2d},\qquad Y(t)=D_zS_t(z).
$$

The [Jacobi determinant derivative formula](../../../../../../jacobi-determinant-derivative-formula.md) gives

$$
J'(t)=\operatorname{tr}(D_zb(t,S_t(z)))J(t)
=(\operatorname{div}_zb)(t,S_t(z))J(t).
$$

The mixed derivatives in the [Hamiltonian vector field](../../../../../../hamiltonian-vector-field.md) cancel:

$$
\operatorname{div}_zb
=\sum_{i=1}^d\bigl(\partial_{x_i}\partial_{v_i}H
-\partial_{v_i}\partial_{x_i}H\bigr)=0.
$$

Consequently $J'(t)=0$, and $J(0)=1$ gives **preservation of [phase space](../../../../../../phase-space.md) volume**:

$$
\boxed{\det D_zS_t(z)=1.}
$$

The same argument applies to $\Phi(t,s)$ for every starting time $s$. This is the [Liouville theorem in Hamiltonian mechanics](../../../../../../liouville-s-theorem-hamiltonian.md). Explicit time dependence of $H$ does not affect the cancellation.

## ↑ Ancestors (11)

1. [B](../b.md)
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
