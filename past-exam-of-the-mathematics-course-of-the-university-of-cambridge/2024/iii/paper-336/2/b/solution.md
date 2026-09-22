<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $X=\epsilon x$. The equation becomes

$$
\epsilon^2y_{XX}+k(X)^2y=0,
\qquad
k(X)=1+X^3.
$$

Since $k$ is positive for every $X\geq0$, there is no [classical turning point](../../../../../../classical-turning-point.md). The leading [WKB approximation for a slowly varying oscillator](../../../../../../wkb-approximation-for-a-slowly-varying-oscillator.md) is

$$
y\sim\frac1{\sqrt{k(X)}}
\left[
C_+e^{i\epsilon^{-1}\int_0^Xk(S)dS}
+C_-e^{-i\epsilon^{-1}\int_0^Xk(S)dS}
\right].
$$

The condition $y(0)=0$ selects a sine, and $y_x(0)=1$ fixes its coefficient. Since

$$
\frac1\epsilon\int_0^X(1+S^3)\,dS
=x+\frac{\epsilon^3x^4}{4},
$$

the result is

$$
\boxed{
y(x)\sim
\frac1{\sqrt{1+(\epsilon x)^3}}
\sin\left(x+\frac{\epsilon^3x^4}{4}\right)}.
$$

The WKB validity measure

$$
\epsilon\frac{|k'(X)|}{k(X)^2}
=\epsilon\frac{3X^2}{(1+X^3)^2}
$$

is uniformly $O(\epsilon)$ and tends to zero at both ends of $X\geq0$. With no turning point, the approximation is therefore uniformly valid on the entire stated half-line.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
