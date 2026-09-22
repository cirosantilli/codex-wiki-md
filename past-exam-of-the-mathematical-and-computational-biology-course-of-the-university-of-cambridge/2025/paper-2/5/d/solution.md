<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Admissions add to the [expected value](../../../../../expected-value-split.md) at rate $\alpha$, while the expected aggregate discharge rate is $\delta\mathbb E[X(t)]$. Consequently

$$
\boxed{N'(t)=\alpha-\delta N(t)}.
$$

Multiplying this [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md) by the [integrating factor](../../../../../integrating-factor.md) $e^{\delta t}$ gives

$$
\frac{d}{dt}[e^{\delta t}N(t)]=\alpha e^{\delta t}.
$$

Integrating from zero, using $N(0)=0$, gives $e^{\delta t}N(t)=\alpha(e^{\delta t}-1)/\delta$. Hence

$$
\boxed{N(t)=\frac\alpha\delta(1-e^{-\delta t})}.
$$

It starts at zero, has initial slope $\alpha$, and approaches $\alpha/\delta$ as $t\to\infty$, as the admission and discharge rates balance.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
