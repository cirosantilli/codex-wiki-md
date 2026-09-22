<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the standard normalization of the [Hecke operator](../../../../../../hecke-operator.md), for which

$$
a_m(T_nf)=\sum_{r\mid\gcd(m,n)}r^{k-1}a_{mn/r^2}(f),\qquad a_1(T_nf)=a_n(f).
$$

The [Hecke multiplication relations](../../../../../../hecke-multiplication-relations.md) make these operators commute; a coefficient-based proof is included in 3(i). For a [cusp form](../../../../../../cusp-form.md), $a_0(f)=0$, so the preceding coefficient relation says

$$
a_1\left(\left[T_n-\sum_{j=1}^{d-1}c_n(j)T_j\right]f\right)=0
$$

for every $f\in S_k$. Denote the bracketed operator by $D_n$. A vanishing first coefficient alone would not prove $D_n=0$. Instead, for every $m\geq1$, commute it past $T_m$ and apply the same relation to the cusp form $T_mf$:

$$
a_m(D_nf)=a_1(T_mD_nf)=a_1(D_nT_mf)=0.
$$

Its constant coefficient is zero too. Thus every Fourier coefficient of $D_nf$ vanishes, and holomorphy gives $D_nf=0$. We have proved

$$
\boxed{T_n=\sum_{j=1}^{d-1}c_n(j)T_j\quad\text{on }S_k.}
$$

For $n\geq d$ these are the integers constructed in (ii); for $1\leq n<d$, the extension $c_n(j)=\delta_{nj}$ makes the formula tautological. Without that implicit extension the symbols in the printed all-index assertion are undefined. The $j=0$ term is excluded because its coefficient functional is zero on cusp forms. If $S_k=0$, the operator statement is vacuous. This also exhibits the [perfect integral Hecke pairing](../../../../../../perfect-integral-hecke-pairing.md): the first $d-1$ coefficient functionals on the cusp space are dual to $T_1,\ldots,T_{d-1}$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
