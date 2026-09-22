<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The feature space may be extremely high-dimensional or infinite-dimensional, and $\phi$ may be known only implicitly. Instead, compute the leading eigenvector $\alpha$ of the [kernel matrix](../../../../../../kernel-matrix.md) $K$, normalize it by $\alpha^\top K\alpha=1$, and use the [kernel trick](../../../../../../kernel-trick.md):

$$
s(x)=\langle v,\phi(x)\rangle
=\sum_{i=1}^n\alpha_i k(x_i,x).
$$

This requires only kernel evaluations.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
