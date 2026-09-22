<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a deterministic $s>0$, the [positive part](../../../../../../positive-part-of-a-real-valued-function.md) $(s-K)_+$ vanishes for $K\ge s$, so direct integration gives

$$
\int_0^\infty K^{\varepsilon-1}(s-K)_+\,dK
=s\frac{s^\varepsilon}{\varepsilon}-\frac{s^{1+\varepsilon}}{1+\varepsilon}
=\frac{s^{1+\varepsilon}}{\varepsilon(1+\varepsilon)}.
$$

At $s=0$ both sides vanish. Applying this pointwise to the nonnegative random variable proves the [power payoff static call representation](../../../../../../power-payoff-static-call-representation.md)

$$
\boxed{S^{1+\varepsilon}=\varepsilon(1+\varepsilon)\int_0^\infty K^{\varepsilon-1}(S-K)_+\,dK.}
$$

By [Tonelli theorem](../../../../../../tonelli-theorem.md), the corresponding moment identity is

$$
M(1+\varepsilon)=\varepsilon(1+\varepsilon)\int_0^\infty K^{\varepsilon-1}C(K)\,dK,
$$

including the possibility that both sides are infinite. No higher-moment assumption is needed to interchange these nonnegative integrals.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
