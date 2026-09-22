<h1 id="2/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply the [Frobenius characteristic map](../../../../../../../frobenius-characteristic-map.md). For even $n$, the [Jacobi–Trudi identity](../../../../../../../jacobi-trudi-identity.md) and cancellation of consecutive terms give

$$
\operatorname{ch}(F)
=\sum_{r=0}^{n}(-1)^r h_{n-r}h_r
=[t^n]H(t)H(-t).
$$

The generating function for the [complete homogeneous symmetric polynomials](../../../../../../../complete-homogeneous-symmetric-polynomial.md) now gives

$$
H(t)H(-t)
=\exp\left(\sum_{j\geq1}\frac{p_jt^j}{j}\right)
 \exp\left(\sum_{j\geq1}\frac{(-1)^jp_jt^j}{j}\right)
=\exp\left(\sum_{j\geq1}\frac{p_{2j}t^{2j}}{j}\right).
$$

This expansion contains only products $p_\mu$ for which every part of $\mu$ is even. The coefficient of $p_\mu$ in $\operatorname{ch}(F)$ is $F(\mu)/z_\mu$, so $F(\mu)=0$ whenever the cycle type $\mu$ has an odd part. Equivalently, $F(g)=0$ whenever $g$ contains an odd cycle. This is the [Two-row alternating character cancellation](../../../../../../../two-row-alternating-character-cancellation.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [Paper 160](../../../../paper-160-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
