<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the nondegenerate restriction of the [Killing form](../../../../../../killing-form.md) to $\mathfrak t$ to define $t_\alpha\in\mathfrak t$ by

$$
\kappa(t_\alpha,t)=\alpha(t)
\qquad(t\in\mathfrak t).
$$

Killing-form invariance and the [root-space decomposition](../../../../../../root-space-decomposition.md) show that $\mathfrak g_\alpha$ pairs nondegenerately with $\mathfrak g_{-\alpha}$ and orthogonally with every other root space. Choose nonzero $e\in\mathfrak g_\alpha$ and $f\in\mathfrak g_{-\alpha}$ with $\kappa(e,f)\ne0$. For $t\in\mathfrak t$,

$$
\kappa([e,f],t)=\kappa(e,[f,t])
=\alpha(t)\kappa(e,f),
$$

so

$$
[e,f]=\kappa(e,f)t_\alpha\ne0.
$$

We need $\alpha(t_\alpha)\ne0$. If it were zero, the span of $e,f,t_\alpha$ would be a solvable Heisenberg-type Lie algebra with central commutator $[e,f]$. By [Lie theorem](../../../../../../lie-s-theorem.md), its adjoint action on $\mathfrak g$ can be upper triangularized, so $\operatorname{ad}[e,f]$ is nilpotent. But $[e,f]\in\mathfrak t$, and elements of the [Cartan subalgebra](../../../../../../cartan-subalgebra.md) act semisimply; hence $\operatorname{ad}[e,f]=0$. A semisimple Lie algebra has zero center, contradicting $[e,f]\ne0$.

Set

$$
h_\alpha=\frac{2t_\alpha}{\alpha(t_\alpha)}.
$$

Rescale $f$ so that $[e_\alpha,f_\alpha]=h_\alpha$. Since $e_\alpha$ and $f_\alpha$ lie in the $\alpha$ and $-\alpha$ root spaces,

$$
[h_\alpha,e_\alpha]=2e_\alpha,
\qquad
[h_\alpha,f_\alpha]=-2f_\alpha.
$$

**Thus $\mathfrak m_\alpha=\langle e_\alpha,h_\alpha,f_\alpha\rangle$ is the [sl2 subalgebra associated with a root](../../../../../../sl2-subalgebra-associated-with-a-root.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
