<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With $X=\epsilon x$, the equation is

$$
\epsilon^2y_{XX}+k^2(X)y=0.
$$

The leading [WKB approximation for a slowly varying oscillator](../../../../../../wkb-approximation-for-a-slowly-varying-oscillator.md) is

$$
\boxed{
y\sim\frac1{\sqrt{k(X)}}\left[
C_+e^{iS(X)/\epsilon}+C_-e^{-iS(X)/\epsilon}
\right],
\qquad
S(X)=\int^Xk(s)ds.}
$$

It requires smooth nonzero $k$, $\epsilon|k'|/|k|^2\ll1$, and distance from every [classical turning point](../../../../../../classical-turning-point.md) large compared with its turning-point scale.

For $k(X)=\sqrt{1+X^2}$,

$$
S(X)=\int_0^X\sqrt{1+s^2}ds
=\frac12\left[X\sqrt{1+X^2}+\operatorname{arsinh}X\right].
$$

Since $k(0)=1$ and $k'(0)=0$, the initial data select the cosine branch without an $O(1)$ phase correction. Hence, for $x>0$ in the WKB regime,

$$
\boxed{
y(x)\sim(1+\epsilon^2x^2)^{-1/4}
\cos\left\{
\frac{\epsilon x\sqrt{1+\epsilon^2x^2}
+\operatorname{arsinh}(\epsilon x)}{2\epsilon}
\right\}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
