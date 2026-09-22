<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Setting the mean equation's derivative to zero gives

$$
\boxed{\widehat N=\frac\alpha\delta=\frac5{0.2}=25\ \text{animals}}.
$$

When the actual current occupancy is $n=25$, the next admission has [exponential distribution](../../../../../exponential-distribution.md) rate five and the next discharge has rate $n\delta=5$. The [memoryless property](../../../../../memorylessness-of-the-exponential-distribution.md) makes these independent competing clocks conditional on the current occupancy. Therefore

$$
\boxed{P(\text{discharge before admission}\mid X=25)=\frac{25(0.2)}{5+25(0.2)}=\frac12}.
$$

The rate comparison uses the actual stated occupancy. Knowing only the mean occupancy would not justify replacing the random $X$ inside $X\delta/(\alpha+X\delta)$ by its mean.

## ↑ Ancestors (13)

1. [E](../e.md)
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
