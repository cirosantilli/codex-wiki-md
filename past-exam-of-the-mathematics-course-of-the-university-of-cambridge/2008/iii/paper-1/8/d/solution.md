<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

One implication is immediate: a unitary module equivalence makes each space an isometric copy of the entire other space, which is closed and invariant. For the converse, choose isometric intertwiners $u:H_1\to H_2$ and $v:H_2\to H_1$ supplied by the two embeddings. Their ranges are closed reducing subspaces. We construct the unitary, proving the [Schröder-Bernstein theorem for Hilbert space modules](../../../../../../schroder-bernstein-theorem-for-hilbert-space-modules.md) in this setting.

Put $w=vu$, an isometric intertwiner of $H_1$ into itself, and let $D=H_1\ominus vH_2$. The spaces $w^nD$, $n\geq0$, are mutually orthogonal. For $m>n$, applying the isometry relation reduces their [inner product](../../../../../../inner-product.md) to one between $D$ and $w^{m-n}D\subseteq wH_1\subseteq vH_2$, which is zero. Hence

$$
K=\bigoplus_{n\geq0}w^nD
$$

is a closed reducing submodule of $H_1$, and $K=D\oplus wK$. Its [orthogonal complement](../../../../../../orthogonal-complement.md) lies in $vH_2$, because it is orthogonal to $D$. Combining these decompositions gives

$$
vH_2=wK\oplus K^\perp.
$$

Apply the inverse isometry $v^*$ on $vH_2$ to obtain

$$
H_2=uK\oplus v^*K^\perp.
$$

The operator

$$
\boxed{W\xi=u\xi\quad(\xi\in K),\qquad
W\xi=v^*\xi\quad(\xi\in K^\perp)}
$$

is therefore an isometry onto $H_2$: it is isometric on each orthogonal summand and their images are the two orthogonal summands just exhibited. Both pieces intertwine the action of $M$, as do the [projections](../../../../../../projection-linear-algebra.md) onto $K$ and $K^\perp$, so $W$ is a unitary module equivalence. This proves the reverse implication with no finiteness assumption on either module.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
