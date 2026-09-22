<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The outer expansion behaves as $f\sim x^{-1}$ near zero. The terms $x$ and $\epsilon f$ become comparable when $x^2=O(\epsilon)$, so

$$
\boxed{x=\sqrt\epsilon X,
\qquad f=\epsilon^{-1/2}F(X).}
$$

The equation has the exact first integral

$$
xf+\frac\epsilon2f^2=x^2+1+2\epsilon,
$$

where the constant follows from $f(1)=2$. Thus

$$
XF+\frac12F^2=1+\epsilon(X^2+2).
$$

Writing $F=F_0+\epsilon F_1+\cdots$ and choosing the branch matching the positive outer solution gives

$$
F_0=\sqrt{X^2+2}-X,
\qquad
F_1=\sqrt{X^2+2}.
$$

Hence

$$
\boxed{f(x)\sim\epsilon^{-1/2}[\sqrt{X^2+2}-X]
+\epsilon^{1/2}\sqrt{X^2+2},
\qquad X=\frac x{\sqrt\epsilon}.}
$$

Its large-$X$ expansion matches the supplied outer series.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
