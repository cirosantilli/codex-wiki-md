<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Weyl-von Neumann theorem](../../../../../../weyl-von-neumann-theorem.md) states that on a separable [Hilbert space](../../../../../../hilbert-space-split.md) a [self-adjoint operator](../../../../../../self-adjoint-operator.md) is a diagonal [self-adjoint operator](../../../../../../self-adjoint-operator.md) plus a compact [self-adjoint operator](../../../../../../self-adjoint-operator.md). For a bounded operator $T$, the perturbation can in fact be chosen Hilbert-Schmidt with arbitrarily small [Hilbert-Schmidt norm](../../../../../../hilbert-schmidt-norm.md). The separable-space formulation is also recorded in [Kadison's Corollary B](https://www.isibang.ac.in/~soumyashant/misc/collected-works-of-kadison/1980s/1988_The_Weyl_theorem_and_block_decompositions.pdf).

Here is a constructive proof. The bounded self-adjoint spectral theorem decomposes a separable $H$ into countably many cyclic reducing spaces, on each of which $T$ is multiplication by $x$ in $L^2(\mu)$ for a finite measure supported in a bounded real interval. First work on one such space. Partition the interval into $N$ intervals of length at most $\delta$, and repeatedly bisect them. Let $E_j$ be the finite-dimensional space of functions constant on the level-$j$ intervals. These spaces are nested and their union is dense, since dyadic step functions approximate continuous functions and continuous functions are dense in $L^2(\mu)$.

Choose normalized interval indicators as a basis of $E_0$, and choose [orthonormal bases](../../../../../../orthonormal-basis.md) of $E_j\ominus E_{j-1}$ within each parent interval. This is possible because the refinement splits into orthogonal parent blocks. Each new basis vector at level $j\geq1$ is supported in an interval of length at most $\delta2^{-(j-1)}$, and there are at most $N2^{j-1}$ such vectors. For every basis vector $e$ choose a real $\lambda_e$ in its supporting interval and define the diagonal operator $De=\lambda_e e$. Then

$$
\|(T-D)e\|\leq\text{length of its supporting interval},
$$

so

$$
\|T-D\|_{\mathrm{HS}}^2
=\sum_e\|(T-D)e\|^2
\leq N\delta^2+\sum_{j\geq1}N2^{j-1}\delta^22^{-2(j-1)}
=3N\delta^2.
$$

One may take $N=O(\delta^{-1})$, so this bound tends to zero as $\delta\to0$. The error is Hilbert-Schmidt, hence compact; it is self-adjoint because both $T$ and $D$ are.

On the countably many cyclic summands choose error bounds $\varepsilon_j$ with $\sum_j\varepsilon_j^2<\varepsilon^2$. Combining their [orthonormal bases](../../../../../../orthonormal-basis.md) and diagonal operators gives $T=D+K$ with $\|K\|_{\mathrm{HS}}<\varepsilon$, proving the assertion. For an unbounded [self-adjoint operator](../../../../../../self-adjoint-operator.md), first split by spectral intervals $[j,j+1)$, apply the bounded construction on each, and choose summable error bounds. The resulting total $K$ is bounded compact, and $D=T-K$ has the same domain as $T$; the diagonal domain condition follows from the boundedness of $K$.

Separability matters. Take an uncountable orthogonal sum of copies of multiplication by $x$ on $L^2[0,1]$. The range closure of a [compact operator](../../../../../../compact-operator-split.md) is separable, and a separable subspace of this direct sum is supported in only countably many summands: choose a countable dense set and unite its countable supports. A self-adjoint compact error therefore vanishes on every remaining summand, each of which reduces the proposed diagonal operator $D=T-K$. The restriction of a diagonal self-adjoint operator to a reducing subspace has pure point spectrum, whereas multiplication by $x$ on $L^2[0,1]$ has no eigenvectors. This is a contradiction, qualifying the theorem if the unspoken separability convention is dropped.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
