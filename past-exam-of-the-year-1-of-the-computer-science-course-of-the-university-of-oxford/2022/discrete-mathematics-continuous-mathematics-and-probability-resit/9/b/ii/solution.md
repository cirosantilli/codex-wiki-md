<h1 id="9/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The same integral works with both powers shifted:

$$
\begin{aligned}
\mathbb E[X^s(1-X)^t]&=\frac{\Gamma(\alpha+\beta)}{\Gamma(\alpha)\Gamma(\beta)}\int_0^1x^{\alpha+s-1}(1-x)^{\beta+t-1}\,\mathrm dx\\
&=\boxed{\frac{\Gamma(\alpha+\beta)\Gamma(\alpha+s)\Gamma(\beta+t)}{\Gamma(\alpha)\Gamma(\beta)\Gamma(\alpha+\beta+s+t)}}.
\end{aligned}
$$

The assumptions $s>-\alpha$ and $t>-\beta$ say precisely that the exponents at each endpoint are greater than $-1$, ensuring [integrability](../../../../../../integrability.md) there. Values of a negative power at the endpoints themselves can be assigned arbitrarily, because those endpoints have [probability](../../../../../../probability.md) zero. This establishes the [mixed power moments of a beta distribution](../../../../../../mixed-power-moments-of-a-beta-distribution.md) without requiring $s$ and $t$ to be [integers](../../../../../../integer-split.md).[NIST DLMF §5.12, equation 5.12.1](../../../../../../nist-digital-library-of-mathematical-functions/5-12-beta-function.md)

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
