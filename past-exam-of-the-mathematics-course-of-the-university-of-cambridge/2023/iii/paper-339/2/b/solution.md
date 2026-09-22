<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $T(w)=w$, the defining equation becomes $M(w)+F(w)=M(w)$, so $\boxed{F(w)=0}$.

A map is [firmly nonexpansive](../../../../../../firmly-nonexpansive-mapping.md) in the $M$-inner product when

$$
\|T(v)-T(w)\|_M^2
\leq\langle T(v)-T(w),v-w\rangle_M.
$$

Put $p=T(v)$ and $q=T(w)$. The two implicit equations give

$$
F(p)=M(v-p),\qquad F(q)=M(w-q).
$$

Because $F$ is a [monotone operator](../../../../../../monotone-operator.md),

$$
0\leq\langle F(p)-F(q),p-q\rangle
=\langle(v-w)-(p-q),p-q\rangle_M.
$$

Therefore

$$
\boxed{
\|p-q\|_M^2
\leq\langle p-q,v-w\rangle_M,}
$$

which is precisely firm nonexpansiveness. In particular, the [preconditioned proximal point algorithm](../../../../../../preconditioned-proximal-point-algorithm.md) map $T=(M+F)^{-1}M$ is [nonexpansive](../../../../../../nonexpansive-mapping.md) in the norm induced by the [positive-definite matrix](../../../../../../positive-definite-matrix.md) $M$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
