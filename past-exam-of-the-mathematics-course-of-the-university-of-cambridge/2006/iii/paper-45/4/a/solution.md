<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use standard neutral coalescent time units, so each pair of ancestral lineages merges at rate 1. With $j$ lineages, there are $\binom j2$ possible pairs; consequently the successive waiting times are independent with

$$
T_j\sim\operatorname{Exp}(\lambda_j),\qquad \lambda_j=\frac{j(j-1)}2.
$$

During this epoch there are $j$ branches, each of length $T_j$. Hence the [total branch length of a neutral coalescent](../../../../../../total-branch-length-of-a-neutral-coalescent.md) is $L=\sum_{j=2}^n jT_j$, and [linearity of expectation](../../../../../../linearity-of-expectation.md) gives

$$
\boxed{EL=\sum_{j=2}^n\frac{j}{\lambda_j}=2\sum_{i=1}^{n-1}\frac1i.}
$$

The root branch above the sample's common ancestor is excluded: its mutations would be shared by every chromosome and would not be [segregating sites](../../../../../../segregating-site.md) in the sample.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
