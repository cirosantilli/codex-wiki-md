<h1 id="7h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $g(0)=0$. [First-step analysis](../../../../../../first-step-analysis.md) gives

$$
 g(1)=1+\frac12g(2),
$$



$$
 g(2)=1+\frac12g(1)+\frac12g(3),
$$

and, because state $3$ moves to $2$ or remains at $3$ with equal probabilities,

$$
 g(3)=1+\frac12g(2)+\frac12g(3).
$$

The last equation gives $g(3)=2+g(2)$. Substitution into the second gives $g(2)=4+g(1)$, and the first then gives $g(1)=3+g(1)/2$. Hence

$$
\boxed{g(1)=6,\qquad g(2)=10,\qquad g(3)=12}.
$$

These are the [expected hitting times](../../../../../../expected-hitting-time.md) of the absorbing state.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7H](../../7h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
