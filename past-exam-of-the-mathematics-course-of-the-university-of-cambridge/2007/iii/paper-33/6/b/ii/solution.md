<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Refining an occupied cell replaces it by two child cells, at least one of which is occupied. All children of a cell contained in $J$ remain contained in $J$, and additional cells can enter the sum. Hence $M_n(J)$ is nondecreasing, pathwise, and is at most $M(J)$.

We must also address boundary points for a fixed interval $J$. For every fixed deterministic $x$, take bounded intervals $I_r$ containing $x$ with lengths tending to zero. The assumed void law gives

$$
\mathbb P(M(\{x\})>0)\leq\mathbb P(M(I_r)>0)=1-e^{-\lambda(I_r)}\longrightarrow0.
$$

Thus the fixed endpoints of $J$ are almost surely not atoms. This is the [exponential void probabilities forbid fixed atoms](../../../../../../../exponential-void-probabilities-forbid-fixed-atoms.md) observation; it is not a simultaneous assertion for all possible real endpoints.

In a fixed bounded interval containing $J$, local finiteness gives only finitely many atoms. Simplicity makes their locations distinct, so there is a positive minimum distance between any two, unless there is at most one. Every atom in the interior of $J$ also has positive distance from its endpoints. For sufficiently fine dyadic cells each such atom lies alone in a cell fully contained in $J$, including if the atom itself is at a dyadic boundary because the cells are half-open. Thus the [dyadic occupancy approximation of a simple point measure](../../../../../../../dyadic-occupancy-approximation-of-a-simple-point-measure.md) eventually equals $M(J)$, almost surely. In particular,

$$
\boxed{M_n(J)\uparrow M(J)\quad\text{almost surely}.}
$$

The union of fully contained level-$n$ cells misses at most two boundary portions of total length at most $2^{1-n}$. Consequently $N_n2^{-n}\to\lambda(J)$, and $p_n/2^{-n}\to1$. For $0\leq z\leq1$, the [probability generating function](../../../../../../../probability-generating-function.md) from the binomial calculation gives

$$
\mathbb E[z^{M_n(J)}]=(1+p_n(z-1))^{N_n}\longrightarrow\exp(\lambda(J)(z-1)).
$$

The convergence follows by expanding the logarithm, since $N_np_n\to\lambda(J)$ and $N_np_n^2\to0$. Since the counts converge almost surely, bounded convergence identifies the same expression as $\mathbb E[z^{M(J)}]$. It is the generating function of the [Poisson distribution](../../../../../../../poisson-distribution.md), whose power-series coefficients determine its law. Thus

$$
\boxed{M(J)\sim\operatorname{Poisson}(\lambda(J)).}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
