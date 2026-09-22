<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

The nonzero [leading coefficients](../../../../../leading-coefficient-of-a-polynomial.md) and distinct degrees make $P_0,\ldots,P_{n-1}$ a [basis](../../../../../basis.md) of the [polynomials](../../../../../polynomial-split.md) of degree at most $n-1$. Consequently the given [orthogonality](../../../../../orthogonal-vectors.md) implies $\int_a^bf(x)Q(x)dx=0$ for every such [polynomial](../../../../../polynomial-split.md) $Q$.

If $f$ has infinitely many distinct zeros in $(a,b)$, there is nothing to prove. Otherwise suppose it has fewer than $n$. Among those zeros, list the sign-changing ones as $t_1<\cdots<t_m$, with $m<n$, and put $Q(x)=\prod_{j=1}^m(x-t_j)$, using $Q=1$ when $m=0$. On each interval between zeros, $f$ has a fixed sign by [continuity](../../../../../continuous-function.md). Crossing a sign-changing zero flips both $f$ and $Q$; crossing any other zero flips neither sign. Thus $fQ$ has one constant sign wherever nonzero. Since $f$ is not identically zero, [continuity](../../../../../continuous-function.md) gives an [open interval](../../../../../open-interval.md) on which $fQ$ is strictly of that sign. Hence its integral is nonzero, contrary to orthogonality to $Q$. **Therefore $f$ has at least $n$ distinct zeros in $(a,b)$.** This is the reusable [orthogonality forces many interior zeros](../../../../../orthogonality-forces-many-interior-zeros.md) argument.

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
