<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

Choose $z=e^{it}$ on the right semicircle, with the continuous branch $\log z=it$. Then

$$
I=\frac1i\int_{-i}^{i}\frac{z^u}{z+iA}\,dz.
$$

Here the integral is along that semicircle. Since $|A|>1$, the pole lies outside the unit disc and the [geometric series](../../../../../geometric-series.md) converges uniformly on the contour.

Put

$$
H_u(w)={}_2F_1(1,u+1;u+2;w).
$$

The [Euler integral for the hypergeometric function](../../../../../euler-integral-for-the-hypergeometric-function.md), initially for $\operatorname{Re}u>-1$, gives

$$
H_u(w)=(u+1)\int_0^1\frac{s^u}{1-ws}\,ds
=(u+1)\sum_{n\ge0}\frac{w^n}{u+n+1},\qquad |w|<1.
$$

The prefactor follows from $\Gamma(u+2)/\Gamma(u+1)=u+1$. Hence an antiderivative of the contour integrand before multiplication by $1/i$ is

$$
\frac{z^{u+1}}{iA(u+1)}H_u\!\left(-\frac z{iA}\right).
$$

Evaluating at the endpoints with the chosen branch yields

$$
\boxed{I(u,A)=
-\frac{i}{A(u+1)}
\left[
e^{i\pi u/2}{}_2F_1(1,u+1;u+2;-1/A)
+e^{-i\pi u/2}{}_2F_1(1,u+1;u+2;1/A)
\right].}
$$

This is first obtained where the individual expressions are defined. The original finite-interval integral is entire in $u$, so [analytic continuation](../../../../../analytic-continuation.md) gives the result elsewhere, taking removable limits at the apparent exceptional negative integers. That convention matters: the two separate hypergeometric terms may be singular even though their combination is finite.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
