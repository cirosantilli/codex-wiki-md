<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $f$ is a modular function that is holomorphic on $\mathfrak h$, it has a Laurent expansion

$$
f(\tau)=\sum_{n\geq-N}a_nq^n
$$

with a finite principal part at infinity. The [Hecke operator on modular forms](../../../../../../hecke-operator.md) acts on this expansion by

$$
T_pf=\sum_n\left(a_{pn}+p^{k-1}a_{n/p}\right)q^n.
$$

If $N>0$ and $a_{-N}\ne0$, the term $p^{k-1}f(p\tau)$ shows that $T_pf$ has pole order $pN$. Inductively, $T_p^rf$ has pole order $p^rN$ with nonzero leading coefficient. Functions with distinct pole orders are [linearly independent](../../../../../../linear-independence.md), so

$$
f,T_pf,T_p^2f,\ldots
$$

would span an infinite-dimensional vector space. This contradicts the hypothesis. Hence $N=0$, and $f$ is holomorphic at infinity. Together with its assumed holomorphy on $\mathfrak h$, this proves that $f$ is a modular form, as asserted by the [finite Hecke orbit criterion for holomorphy at a cusp](../../../../../../finite-hecke-orbit-criterion-for-holomorphy-at-a-cusp.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
