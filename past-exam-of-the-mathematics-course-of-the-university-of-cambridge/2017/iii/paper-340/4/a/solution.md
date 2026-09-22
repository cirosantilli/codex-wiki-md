<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For real $u\in L^1(\Omega)$, its [total variation seminorm on a domain](../../../../../../total-variation-seminorm-on-a-domain.md) is

$$
\boxed{|Du|(\Omega)=\sup\left\{\int_\Omega u\,\operatorname{div}\xi\,dx:\xi\in C_c^1(\Omega;\mathbb R^2),\ |\xi(x)|_2\le1\right\}.}
$$

The [vector fields](../../../../../../vector-field.md) have [compact support](../../../../../../compact-support.md) inside $\Omega$, so no boundary term is charged. Taking both $\xi$ and $-\xi$ makes this equivalent to a supremum of absolute pairings. When finite, the [distributional derivative](../../../../../../distributional-derivative.md) $Du$ is a finite vector-valued [Radon measure](../../../../../../radon-measure.md), and the displayed supremum is its [total variation norm of a measure](../../../../../../total-variation-norm-of-a-measure.md). For a [smooth](../../../../../../smooth-function.md) [function](../../../../../../function-split.md) it equals $\int_\Omega|\nabla u|_2\,dx$.

The [function of bounded variation on a domain](../../../../../../function-of-bounded-variation-on-a-domain.md) belongs to the [Banach space](../../../../../../banach-space-split.md)

$$
\boxed{BV(\Omega)=\{u\in L^1(\Omega):|Du|(\Omega)<\infty\},\qquad\|u\|_{BV}=\|u\|_{L^1}+|Du|(\Omega).}
$$

The [L1 norm](../../../../../../l1-norm.md) is needed because variation alone vanishes on constant [functions](../../../../../../function-split.md) and is only a [seminorm](../../../../../../seminorm.md). No smoothness of $u$ is part of this definition.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
