<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $F=(1-\epsilon)\Phi+\epsilon H$ and assume $0<\epsilon<1/2$. If $m$ is its median, then

$$
\frac{1/2-\epsilon}{1-\epsilon}
\leq\Phi(m)\leq
\frac1{2(1-\epsilon)}.
$$

Moreover its density satisfies $f(m)\geq(1-\epsilon)\phi(m)$. Since the [standard normal density](../../../../../../standard-normal-density.md) decreases with $|m|$, the smallest possible density at the median occurs at either endpoint. Put

$$
q_\epsilon=\Phi^{-1}\!\left(\frac1{2(1-\epsilon)}\right)>0.
$$

The two endpoints are $\pm q_\epsilon$ by normal symmetry. The bound is attained by choosing a contaminating density supported strictly to the right of $q_\epsilon$, or symmetrically to the left of $-q_\epsilon$, with zero density at the selected median. Therefore

$$
\boxed{\max_{F\in\mathcal P_\epsilon(\Phi)}A(T,F)
=\frac1{4(1-\epsilon)^2\phi(q_\epsilon)^2}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
