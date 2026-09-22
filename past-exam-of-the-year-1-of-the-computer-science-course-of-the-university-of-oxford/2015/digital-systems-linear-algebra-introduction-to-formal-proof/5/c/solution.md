<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The smallest positive normal [half-precision floating-point number](../../../../../half-precision-floating-point-format.md) uses $E=1$ and a zero fraction, while the largest uses $E=30$ and all ten fraction [bits](../../../../../bit.md) equal to one. Hence

$$
\boxed{x_{\min,\mathrm{normal}}=1.0_2\,2^{1-15}=2^{-14},\qquad x_{\max,\mathrm{normal}}=(2-2^{-10})2^{15}=65504.}
$$

The corresponding words are `0 00001 0000000000` and `0 11110 1111111111`. The stored [exponent](../../../../../exponent.md) $31$ is reserved and cannot extend the finite normal range.

For a [subnormal number](../../../../../subnormal-number.md), $E=0$ and the implicit leading [bit](../../../../../bit.md) becomes zero, while the scale remains $2^{1-15}=2^{-14}$. The least positive nonzero fraction is $0.0000000001_2=2^{-10}$, giving

$$
\boxed{x_{\min,\mathrm{subnormal}}=2^{-10}2^{-14}=2^{-24},\qquad\text{word }0\;00000\;0000000001.}
$$

Using scale $2^{-15}$ here would be incorrect: the [subnormal number](../../../../../subnormal-number.md) convention uses the minimum normal scale, not the ordinary biased-[exponent](../../../../../exponent.md) formula at $E=0$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
