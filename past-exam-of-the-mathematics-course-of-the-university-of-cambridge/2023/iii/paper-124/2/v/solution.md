<h1 id="2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Let a monotone circuit of size $M$ compute the $m$-clique function, and let $\widetilde S=\langle A\rangle$ be its lattice approximation from part (i). If $\widetilde S$ is not universal, part (ii) says that it misses at least half of all positive $m$-cliques. The approximation lemma and part (iii) then imply

$$
\frac12\leq M\cdot4\,2^{-l/2},
\qquad
M\geq2^{l/2}/8.
$$

If $\widetilde S$ is universal, every complete $(m-1)$-partite graph is a negative input that must be covered by a union-error set. Part (iv) gives

$$
1\leq M n^l2^{-r},
\qquad
M\geq2^r/n^l.
$$

Therefore

$$
M\geq
\min\left\{\frac{2^{l/2}}8,\frac{2^r}{n^l}\right\}.
$$

Choose

$$
m=\Theta\!\left((n/\log n)^{2/3}\right),\quad
l=\Theta(\sqrt m),\quad
r=\Theta(n/m),
$$

with constants satisfying the two hypotheses and $r>2l\log_2n$. Both lower bounds are then

$$
\exp\!\left(\Omega((n/\log n)^{1/3})\right).
$$

Since the graph has $\binom n2$ input variables, this is exponential in a positive power of the number of inputs, up to a logarithmic factor.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [2](../../2.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
