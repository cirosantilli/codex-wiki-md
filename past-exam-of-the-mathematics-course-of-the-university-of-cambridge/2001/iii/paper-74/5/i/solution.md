<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $R=\mathcal O_k$, $S=\mathcal O_L$, $T=\mathcal O_K$, and denote their relative [codifferents](../../../../../../inverse-different.md) by $C_{L/k}$, $C_{K/L}$ and $C_{K/k}$. Transitivity of the [field trace](../../../../../../field-trace.md) gives

$$
x\in C_{K/k}\quad\Longleftrightarrow\quad\operatorname{Tr}_{K/L}(xT)\subseteq C_{L/k}.
$$

For the forward direction, testing an element $t\in T$ against every $s\in S$ is legitimate because $st\in T$. For the reverse direction, take $s=1$ and use trace transitivity.

Localize at a nonzero base [prime ideal](../../../../../../prime-ideal.md). The intermediate ring is semilocal [Dedekind domain](../../../../../../dedekind-domain.md), so its invertible [fractional ideal](../../../../../../fractional-ideal.md) $C_{L/k}$ is principal there, say $C_{L/k}=d^{-1}S$ locally. This principality follows by choosing, with the [Chinese remainder theorem for ideals](../../../../../../chinese-remainder-theorem-for-ideals.md), a generator at each of its finitely many maximal ideals. The displayed criterion now becomes

$$
x\in C_{K/k}\quad\Longleftrightarrow\quad dx\in C_{K/L},\qquad C_{K/k}=d^{-1}C_{K/L}=C_{K/L}C_{L/k}T.
$$

Invert these [fractional ideals](../../../../../../fractional-ideal.md) using Solution 1. Equality at every base localization gives the global [different in a tower](../../../../../../different-in-a-tower.md) formula

$$
\boxed{\mathfrak D_{K/k}=\mathfrak D_{K/L}\bigl(\mathfrak D_{L/k}\mathcal O_K\bigr).}
$$

The second factor is extended to the upper [ring of integers](../../../../../../ring-of-integers.md); that extension is implicit in the printed formula. At a local prime the exponents consequently satisfy $d(K/k)=d(K/L)+e(K/L)d(L/k)$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
