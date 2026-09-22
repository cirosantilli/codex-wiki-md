<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the unit-scale [Laplace distribution](../../../../../../laplace-distribution.md), integrating separately over the two half-lines gives the [moment-generating function](../../../../../../moment-generating-function.md)

$$
M(t)=\frac12\int_0^\infty e^{-(1-t)x}\,dx
+\frac12\int_{-\infty}^0e^{(1+t)x}\,dx
=\frac1{2(1-t)}+\frac1{2(1+t)}
=\frac1{1-t^2},
$$

for $|t|<1$; the appropriate half-line integral diverges outside that interval. Therefore

$$
\boxed{K(t)=-\log(1-t^2),\qquad |t|<1.}
$$

Its derivatives needed for the [saddlepoint density approximation](../../../../../../saddlepoint-density-approximation.md) are

$$
K'(t)=\frac{2t}{1-t^2},\qquad
K''(t)=\frac{2(1+t^2)}{(1-t^2)^2}.
$$

Set $D=\sqrt{1+y^2}$. Solving $K'(\widehat t)=y$ and selecting the root in $(-1,1)$ gives the stable formula

$$
\widehat t=\frac{y}{1+D},
$$

including $\widehat t=0$ at $y=0$. The other quadratic root is outside the domain. At the correct saddlepoint,

$$
1-\widehat t^2=\frac2{1+D},\qquad
\widehat t y=D-1,\qquad
K''(\widehat t)=D(1+D).
$$

Substitution gives the [saddlepoint density of a Laplace sample mean](../../../../../../saddlepoint-density-of-a-laplace-sample-mean.md):

$$
\boxed{\widehat f_{\bar Y}(y)=
\sqrt{\frac{n}{2\pi D(1+D)}}
\exp\!\left[n\left\{\log\frac{1+D}{2}-D+1\right\}\right],
\quad D=\sqrt{1+y^2}.}
$$

It is symmetric in $y$, as the underlying [Laplace distribution](../../../../../../laplace-distribution.md) requires. At zero its value is $\sqrt{n/(4\pi)}$, consistent with the local [normal approximation](../../../../../../normal-approximation.md) having [variance](../../../../../../variance-split.md) $2/n$. This is an approximation, not an exact finite-$n$ density or an automatically normalized one.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
