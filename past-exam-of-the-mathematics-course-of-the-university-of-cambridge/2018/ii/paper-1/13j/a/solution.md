<h1 id="13j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Writing $S_i(t)=1-F_i(t)$ for the [survival function](../../../../../../survival-function.md), the definition of the [hazard function](../../../../../../hazard-function.md) gives

$$
h_i(t)=\frac{f_i(t)}{S_i(t)}
=-\frac{S_i'(t)}{S_i(t)}
=-\frac d{dt}\log S_i(t).
$$

Since $S_i(0)=1$, integration yields

$$
S_i(t)=\exp\left[-\int_0^t h_i(s)\,ds\right].
$$

Therefore

$$
\boxed{\ F_i(t)=1-\exp\left[-\int_0^t h_i(s)\,ds\right]\ }.
$$

The exponent is the negative [cumulative hazard](../../../../../../cumulative-hazard-function.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13J](../../13j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
