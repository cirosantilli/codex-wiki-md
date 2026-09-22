<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The map $\Lambda$ is a [completely positive map](../../../../../../completely-positive-map.md) when $\Lambda\otimes\operatorname{id}_m$ maps positive operators to positive operators for every $m$. In a basis $\{|i\rangle\}$ define the unnormalized [Choi matrix](../../../../../../choi-matrix.md)

$$
J(\Lambda)=\sum_{i,j}|i\rangle\langle j|\otimes\Lambda(|i\rangle\langle j|).
$$

If $\Lambda$ is completely positive, $J(\Lambda)=(\operatorname{id}\otimes\Lambda)(|\Omega\rangle\langle\Omega|)\geq0$, where $|\Omega\rangle=\sum_i|ii\rangle$. Conversely, decompose $J=\sum_k|a_k\rangle\langle a_k|$ and reshape each vector into an operator $A_k$. The Choi reconstruction formula gives $\Lambda(X)=\sum_kA_kXA_k^\dagger$, which is completely positive. Thus

$$
\boxed{\Lambda\text{ is completely positive}\iff J(\Lambda)\geq0}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
