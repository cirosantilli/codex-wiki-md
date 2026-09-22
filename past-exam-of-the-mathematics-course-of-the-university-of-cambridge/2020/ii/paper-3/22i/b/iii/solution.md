<h1 id="22i/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

[Weak-star convergence](../../../../../../../weak-star-topology.md) means pointwise convergence on the predual:

$$
\Lambda_j(x)\longrightarrow\Lambda(x)
\qquad\text{for every }x\in X.
$$

For each $x\in X$, its image $J_Xx\in X''$ under the [canonical embedding into the bidual](../../../../../../../canonical-embedding-into-the-bidual.md) satisfies $(J_Xx)(\Lambda)=\Lambda(x)$. Thus weak convergence implies weak-star convergence, and altogether

$$
\text{norm convergence}\ \Longrightarrow\
\text{weak convergence}\ \Longrightarrow\
\text{weak-star convergence}.
$$

For the requested example, let

$$
f_j(x)=\sin(jx)\in L^\infty(\mathbb R).
$$

The [Riemann-Lebesgue lemma](../../../../../../../riemann-lebesgue-lemma.md) gives $f_j\mathrel{\stackrel{*}{\rightharpoonup}}0$ in $(L^1)'$. Since

$$
f_j(x)^2=\frac12-\frac12\cos(2jx),
$$

the same lemma gives $f_j^2\mathrel{\stackrel{*}{\rightharpoonup}}1/2$. Hence $f=0$ and $g=1/2\ne f^2$, exhibiting the [failure of weak-star convergence to commute with squaring](../../../../../../../failure-of-weak-star-convergence-to-commute-with-squaring.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [22I](../../../22i.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
