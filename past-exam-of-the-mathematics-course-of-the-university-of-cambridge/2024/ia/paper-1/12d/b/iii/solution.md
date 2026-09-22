<h1 id="12d/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $k\geq1$, let $E_k$ be the set of numbers whose first digit $5$ occurs in position $k$. The first $k-1$ digits each have nine allowed values, while the $k$th is fixed, so $E_k$ is a union of decimal intervals of total length

$$
|E_k|=\frac1{10}\left(\frac9{10}\right)^{k-1}.
$$

The set $E_\infty$ of numbers having no digit $5$ can, after $N$ places, be covered by intervals of total length $(9/10)^N$; hence it has length zero.

For each fixed truncation level, the [function](../../../../../../../function-split.md) is constant on finitely many decimal cylinders apart from the remaining set, whose covering length can be made arbitrarily small. The [Riemann integrability criterion](../../../../../../../riemann-integrability-criterion.md) therefore shows that every truncation is Riemann integrable.

For integer $N$,

$$
\int_0^1\min(f,N)\,dx
=\sum_{k=1}^{N-1}
\frac{k}{10}\left(\frac9{10}\right)^{k-1}
+N\left(\frac9{10}\right)^{N-1}.
$$

The final term tends to zero, and monotonicity handles noninteger truncation levels. Therefore the [first occurrence of a decimal digit](../../../../../../../first-occurrence-of-a-decimal-digit.md) calculation gives

$$
\int_0^1f(x)\,dx
=\sum_{k=1}^{\infty}
\frac{k}{10}\left(\frac9{10}\right)^{k-1}
=\frac{1/10}{(1-9/10)^2}
=\boxed{10}.
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [12D](../../../12d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
