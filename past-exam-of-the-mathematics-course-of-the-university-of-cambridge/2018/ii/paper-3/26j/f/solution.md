<h1 id="26j/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Let $|t|<2\alpha$. Both $E$ and its translate $E+t$ lie in an interval of length $1+|t|$. By finite additivity and translation invariance of [Lebesgue measure](../../../../../../lebesgue-measure.md),

$$
m(E\cap(E+t))
=m(E)+m(E+t)-m(E\cup(E+t))
\geq2\left(\frac12+\alpha\right)-(1+|t|)
=2\alpha-|t|>0.
$$

Choose $x\in E\cap(E+t)$. Then $x\in E$ and $x-t\in E$, so $t=x-(x-t)\in E-E$. Therefore the [difference-set overlap bound on an interval](../../../../../../difference-set-overlap-bound-on-an-interval.md) gives

$$
\boxed{(-2\alpha,2\alpha)\subseteq E-E.}
$$

## ↑ Ancestors (11)

1. [F](../f.md)
2. [26J](../../26j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
