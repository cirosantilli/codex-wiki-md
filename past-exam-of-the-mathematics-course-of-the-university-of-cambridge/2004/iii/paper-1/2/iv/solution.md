<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

An [associated prime of a module](../../../../../../associated-prime-of-a-module.md) is an [annihilator](../../../../../../annihilator-ring-theory.md) of a nonzero element. Suppose $Q=\operatorname{Ann}_R(m)$ is prime and $Q\subseteq P$. Then $m/1\ne0$ in $M_P$: a denominator $s\notin P$ killing $m$ would belong to $Q\subseteq P$. Moreover

$$
\operatorname{Ann}_{R_P}(m/1)=QR_P.
$$

Indeed, if $(a/s)(m/1)=0$, some $t\notin P$ has $tam=0$, so $ta\in Q$; primeness and $t\notin Q$ imply $a\in Q$. The reverse containment is immediate. This proves one inclusion in the [localization of associated primes](../../../../../../localization-of-associated-primes.md) formula.

For the other, let $\mathfrak q=\operatorname{Ann}_{R_P}(m/s)$ be an [associated prime](../../../../../../associated-prime-of-a-module.md) of $M_P$ and contract it to $Q$. By part (iii), $Q$ is prime, $Q\subseteq P$ and $QR_P=\mathfrak q$. Since $s$ is invertible, $\mathfrak q$ is also the [annihilator](../../../../../../annihilator-ring-theory.md) of $m/1$. The [Noetherian ring](../../../../../../noetherian-ring.md) hypothesis makes $Q=(a_1,\ldots,a_r)$ finitely generated. For each $a_i$, the equality $(a_im)/1=0$ supplies $t_i\notin P$ with $t_ia_im=0$. Put $t=\prod_i t_i$, taking $t=1$ for the zero [ideal](../../../../../../ideal.md). Then $Q$ annihilates $tm$, while $tm/1\ne0$ because $t/1$ is a [unit](../../../../../../unit-in-a-ring.md) and $m/1\ne0$.

If $b(tm)=0$, then $b/1$ annihilates $m/1$, so $b\in Q$. Therefore $\operatorname{Ann}_R(tm)=Q$, and $Q\in\operatorname{Ass}_R(M)$. We conclude

$$
\boxed{\operatorname{Ass}_{R_P}(M_P)=\{QR_P:Q\in\operatorname{Ass}_R(M),\ Q\subseteq P\}.}
$$

The single common denominator $t$ is the key point: one must turn a localized [annihilator](../../../../../../annihilator-ring-theory.md) into the [annihilator](../../../../../../annihilator-ring-theory.md) of one actual nonzero element of $M$, not merely assert that [annihilators](../../../../../../annihilator-ring-theory.md) commute with [localization](../../../../../../localization-of-a-ring.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
