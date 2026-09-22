<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At weight zero the convention from part (a) is

$$
(T_pF)(\tau)=\frac1p\left(F(p\tau)+\sum_{b=0}^{p-1}F\left(\frac{\tau+b}{p}\right)\right).
$$

Partition the summands of $G$ according to divisibility of the first integer coordinate by $p$. Directly from the definition,

$$
G(p\tau,s)
=p^s\sum_{p\mid m}\frac{y^s}{|m\tau+n|^{2s}}.
$$

In the sum over $b$, the congruence $n\equiv mb\pmod p$ has one solution when $p\nmid m$, has $p$ solutions when $p$ divides both $m$ and $n$, and has none when $p\mid m$ but $p\nmid n$. Therefore

$$
G(p\tau,s)+\sum_{b=0}^{p-1}G\left(\frac{\tau+b}{p},s\right)
=p^sG(\tau,s)+p^{1-s}G(\tau,s),
$$

where the contribution from pairs divisible by $p$ was rescaled by $p^{-2s}$. Dividing by $p$ proves the [Hecke eigenvalue of a nonholomorphic Eisenstein series](../../../../../../hecke-eigenvalue-of-a-nonholomorphic-eisenstein-series.md):

$$
\boxed{T_pG(\tau,s)=(p^{s-1}+p^{-s})G(\tau,s).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
