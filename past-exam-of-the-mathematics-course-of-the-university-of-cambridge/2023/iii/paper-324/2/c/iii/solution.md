<h1 id="2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The ratio $f_i=A_i/B_i$ is the conditional probability that $X$ lies in the left half of interval $i$. After the controlled rotation and uncomputation of $|\theta_i\rangle$, append the rotation qubit to the interval label. The amplitudes become

$$
\sqrt{p_i^{(m)}f_i},|i0\rangle
+\sqrt{p_i^{(m)}(1-f_i)},|i1\rangle.
$$

But

$$
p_i^{(m)}f_i=p_{2i}^{(m+1)},
\qquad
p_i^{(m)}(1-f_i)=p_{2i+1}^{(m+1)}.
$$

Consequently one refinement step maps

$$
|\psi_m\rangle\longmapsto|\psi_{m+1}\rangle.
$$

Starting from $|\psi_1\rangle$ and repeating this [hierarchical probability-distribution state preparation](../../../../../../../hierarchical-probability-distribution-state-preparation.md) for $m=1,\ldots,n-1$ gives

$$
\boxed{|\psi_n\rangle
=\sum_{j=0}^{2^n-1}\sqrt{p_j^{(n)}}|j\rangle}.
$$

There are $n-1=O(\log N)$ refinement levels, each of polylogarithmic size by assumption.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
