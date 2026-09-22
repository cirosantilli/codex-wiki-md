<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Among the nine informative pairs, the active patient fails first once and the placebo patient fails first eight times. The conditional partial likelihood is proportional to

$$
\left(\frac{e^\beta}{1+e^\beta}\right)^1
\left(\frac1{1+e^\beta}\right)^8,
$$

so

$$
e^{\widehat\beta}=\frac18.
$$

Under $H_0$, the number of active-first failures is $\operatorname{Binomial}(9,1/2)$. The exact two-sided [sign test](../../../../../../../sign-test.md) has

$$
p=2\mathbb P\{\operatorname{Binomial}(9,1/2)\leq1\}
=\frac{20}{512}\approx0.0391,
$$

so the data reject at the 5% level and favor lower hazard under active treatment.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
