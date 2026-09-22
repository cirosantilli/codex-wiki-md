<h1 id="9/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Multiply the [probability density function](../../../../../../probability-density-function.md) by $x$ and integrate over its [support](../../../../../../support.md):

$$
\begin{aligned}
\mathbb E[X]&=\frac{\Gamma(\alpha+\beta)}{\Gamma(\alpha)\Gamma(\beta)}\int_0^1x^{\alpha}(1-x)^{\beta-1}\,\mathrm dx\\
&=\frac{\Gamma(\alpha+\beta)}{\Gamma(\alpha)\Gamma(\beta)}\frac{\Gamma(\alpha+1)\Gamma(\beta)}{\Gamma(\alpha+\beta+1)}\\
&=\boxed{\frac{\alpha}{\alpha+\beta}}.
\end{aligned}
$$

The middle equality is the [beta function](../../../../../../beta-function.md) integral with parameters $\alpha+1$ and $\beta$; the last uses the recurrence for the [gamma function](../../../../../../gamma-function.md). Both parameters are positive, so the integral converges. Equivalently, multiplying the [beta distribution](../../../../../../beta-distribution.md) [probability density function](../../../../../../probability-density-function.md) by $x$ converts its kernel to that of a [beta distribution](../../../../../../beta-distribution.md) [probability density function](../../../../../../probability-density-function.md) with its first parameter increased by one.[NIST DLMF §5.12, equation 5.12.1](../../../../../../nist-digital-library-of-mathematical-functions/5-12-beta-function.md)

## ↑ Ancestors (13)

1. [I](../i.md)
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
