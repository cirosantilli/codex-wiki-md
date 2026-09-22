<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

With equal model prior probabilities, [Bayesian model averaging](../../../../../../bayesian-model-averaging.md) gives the unnormalized density

$$
p(H_0\mid D)\propto
\mathbf1_{[H_{0\min},H_{0\max}]}(H_0)
\frac1m\sum_{l=1}^m
\int
\frac{p(\Delta t\mid D)}{\pi_0(\Delta t)}
p(\Delta t\mid H_0,M_l)\,d\Delta t.
$$

Normalizing this expression over the allowed interval automatically incorporates each lens model's evidence and hence its posterior model probability.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
