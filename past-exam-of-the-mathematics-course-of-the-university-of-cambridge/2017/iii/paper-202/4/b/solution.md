<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With the printed assumptions alone, the general [quadratic covariation](../../../../../../quadratic-covariation.md) calculation from the two noise coefficients gives

$$
\begin{aligned}
d[X]&=(X^2+Y^2)\,dt-2XY\,dC,\\
d[Y]&=(X^2+Y^2)\,dt+2XY\,dC,\\
d[X,Y]&=(X^2-Y^2)\,dC.
\end{aligned}
$$

A continuous [finite-variation process](../../../../../../finite-variation-process.md) contributes no [quadratic covariation](../../../../../../quadratic-covariation.md), so the drift terms in the previous part do not alter these formulas. Taking $\vartheta=B$ gives $d[X,Y]=e^{2B}\cos(2B)dt$, which is nonzero near zero since $B_0=0$. Also $d([X]-[Y])=-4XYdt$ is not identically zero. Thus the requested assertions are false as printed.

Under the corrected assumption $C=0$, $X^2+Y^2=e^{2B}$ yields

$$
\boxed{[X]_t=[Y]_t=A_t:=\int_0^te^{2B_s}\,ds,\qquad [X,Y]_t=0.}
$$

The pair is therefore a pair of [orthogonal continuous local martingales](../../../../../../orthogonal-continuous-local-martingales.md). This equality also identifies the clock for the intended [time change of a continuous process](../../../../../../time-change-of-a-continuous-process.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
