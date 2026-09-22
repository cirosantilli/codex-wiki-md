<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $b=\sum_{j=0}^{m-1}2^jb_j$. Applying the [phase gate](../../../../../../../phase-gate.md)

$$
P\left(\frac{2\pi2^j}{Q}\right)
$$

to qubit $b_j$ contributes $\exp(2\pi i2^jb_j/Q)$. The product of these $m$ gates is therefore

$$
\boxed{U|b\rangle=\omega^b|b\rangle}.
$$

Similarly, for $a=\sum_ja_j2^j$ and $b=\sum_kb_k2^k$, apply a [controlled phase gate](../../../../../../../controlled-phase-gate.md)

$$
CP\left(\frac{2\pi2^{j+k}}Q\right)
$$

between every pair $(a_j,b_k)$. The accumulated phase is

$$
\prod_{j,k}\exp\left(\frac{2\pi i}{Q}a_jb_k2^{j+k}\right)
=\omega^{ab}.
$$

The $m^2$ controlled phase gates implement

$$
\boxed{V|a\rangle|b\rangle=\omega^{ab}|a\rangle|b\rangle}.
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
