<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First require $x\neq0$. A [discrete logarithm](../../../../../../../discrete-logarithm-problem.md) to a [generator of a group](../../../../../../../generator-of-a-group.md) of $\mathbb Z_p^*$ exists only for nonzero $x$; the printed membership $x\in\mathbb Z_p$ inadvertently also permits zero, for which $x^{-b}$ is undefined. Zero can be rejected before any [quantum circuit](../../../../../../../quantum-circuit-split.md).

Put $M=p-1$ and write $x=g^y$. Since $g$ is a [generator of a group](../../../../../../../generator-of-a-group.md) of order $M$, the map $k\mapsto g^k$ is a [bijection](../../../../../../../bijection.md) from $\mathbb Z_M$ to the [multiplicative group of a finite field](../../../../../../../multiplicative-group-of-a-finite-field.md). Hence every nonzero $c$ has a unique $k\in\mathbb Z_M$ with $c=g^k$. Equality of powers of $g$ is equality of their exponents modulo $M$, giving

$$
\boxed{f(a,b)=g^{a-by}=c\ \Longleftrightarrow\ a-by\equiv k\pmod M.}
$$

The [fiber](../../../../../../../fiber-of-a-function.md) over $c$ is an affine [coset](../../../../../../../coset.md) of the [subgroup](../../../../../../../subgroup.md) $\{(yb,b):b\in\mathbb Z_M\}$, and contains exactly $M$ pairs. This identifies the [hidden subgroup problem](../../../../../../../hidden-subgroup-problem.md) underlying [discrete-logarithm Fourier sampling](../../../../../../../discrete-logarithm-fourier-sampling.md); knowing $k$ numerically is not needed to construct the [coset state](../../../../../../../coset-state.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
