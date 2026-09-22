<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $x_t=\log S_t$, the [Itô formula](../../../../ito-s-lemma.md) uses $(\log S)'=1/S$ and $(\log S)''=-1/S^2$. Consequently

$$
dx_t=\frac{dS_t}{S_t}-\frac12\frac{d\langle S\rangle_t}{S_t^2}=\left[\alpha(\mu-x_t)-\frac12\sigma^2\right]dt+\sigma\,dZ_t.
$$

The [quadratic variation](../../../../quadratic-variation.md) term shifts the mean level. Thus the [log-mean-reverting price](../../../../log-mean-reverting-price.md) has logarithm following the [Ornstein-Uhlenbeck process](../../../../ornstein-uhlenbeck-process.md)

$$
\boxed{dx_t=\alpha(\widetilde\mu-x_t)dt+\sigma\,dZ_t,\qquad \widetilde\mu=\mu-\frac{\sigma^2}{2\alpha}}.
$$

It is the logarithm, rather than the price itself, which reverts linearly to a constant mean level.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
