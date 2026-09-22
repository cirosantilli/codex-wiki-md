<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Seek an integrating factor $\mu$ such that the differential expression becomes $-(py')'$. Its leading coefficient requires $p=\mu(1-x^2)$, while the first-derivative coefficient requires $-p'=3x\mu$. Thus

$$
(1-x^2)\mu'-2x\mu=-3x\mu,\qquad
\frac{\mu'}\mu=-\frac{x}{1-x^2}.
$$

Choose the positive solution $\mu=\sqrt{1-x^2}$. The [Sturm-Liouville form](../../../../../sturm-liouville-form.md) is therefore

$$
\boxed{-\left[(1-x^2)^{3/2}y_n'\right]'=(n^2-1)\sqrt{1-x^2}\,y_n,}
$$

with

$$
\boxed{p=(1-x^2)^{3/2},\qquad q=0,\qquad w=\sqrt{1-x^2}.}
$$

The weight is positive on the open interval. The endpoints are singular because $p$ vanishes there, but the prescribed boundedness of $y_n,y_n'$ makes the integration-by-parts boundary terms vanish.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
