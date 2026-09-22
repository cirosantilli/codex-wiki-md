<h1 id="11g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because $I$ and $A$ commute, the matrix binomial theorem gives

$$
(I+A)^p=\sum_{j=0}^p\binom pjA^j.
$$

For prime $p$, every intermediate coefficient $\binom pj$ is divisible by $p$, proving the [prime-power binomial congruence for a matrix](../../../../../../prime-power-binomial-congruence-for-a-matrix.md)

$$
(I+A)^p\equiv I+A^p\pmod p.
$$

For

$$
A=\begin{pmatrix}0&-1\\1&0\end{pmatrix},
\qquad A^2=-I,
$$

one has $(I+A)^2=2A$ and $(I+A)^4=-4I$. If $p=4k+1$, then

$$
(I+A)^p=(-4)^k(I+A)
\equiv I+A,
$$

so $(-4)^k\equiv1\pmod p$. If $p=4k-1$, then $A^p=-A$ and

$$
(I+A)^p=(-4)^k(I+A)^{-1}
=\frac{(-4)^k}{2}(I-A)
\equiv I-A,
$$

so $(-4)^k\equiv2\pmod p$.

By [Euler criterion](../../../../../../euler-criterion.md), $(\frac2p)\equiv2^{(p-1)/2}\pmod p$. In either case the preceding congruence gives $(\frac2p)=(-1)^k$. Since $(p^2-1)/8$ has the same parity as $k$ for $p=4k\pm1$, this is the [second supplementary law for quadratic reciprocity](../../../../../../second-supplementary-law-for-quadratic-reciprocity.md)

$$
\boxed{\left(\frac2p\right)=(-1)^{(p^2-1)/8}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11G](../../11g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
