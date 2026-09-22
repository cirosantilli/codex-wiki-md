<h1 id="6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The [space-time Hermite polynomials](../../../../../../space-time-hermite-polynomial.md) obtained by scaling the [Probabilists' Hermite polynomials](../../../../../../probabilists-hermite-polynomial.md) are genuine [polynomials](../../../../../../polynomial-split.md) in both variables, including at $t=0$:

$$
H_n(x,t)=n!\sum_{j=0}^{\lfloor n/2\rfloor}\frac{(-1)^j x^{n-2j}t^j}{2^j j!(n-2j)!}.
$$

This expansion follows by differentiating the defining Gaussian exponential, and shows that $H_n(x,0)=x^n$ extends smoothly through $t=0$. Consequently the [Itô formula](../../../../../../ito-s-lemma.md) is applicable from time zero. The given backward [heat equation](../../../../../../heat-equation.md) cancels the [drift](../../../../../../drift-coefficient.md), and the derivative identity gives

$$
dH_n(B_t,t)=nH_{n-1}(B_t,t)\,dB_t\qquad(n\geq1).
$$

The integrand is continuous and [adapted](../../../../../../adapted-process.md), hence [previsible](../../../../../../predictable-process.md), and stopping the [Brownian motion](../../../../../../brownian-motion-split.md) and time makes it bounded. Thus **$H_n(B_t,t)$ is a [local martingale](../../../../../../local-martingale.md) for every $n\geq0$.** The $n=0$ case is the constant $H_0=1$; in fact Gaussian [moments](../../../../../../moment.md) make the displayed [Itô integral](../../../../../../ito-integral.md) [square-integrable](../../../../../../square-integrable-function.md) on every finite horizon, so these are true [martingales](../../../../../../martingale-split.md) as well.

The first three [Probabilists' Hermite polynomials](../../../../../../probabilists-hermite-polynomial.md) are $h_1(x)=x$, $h_2(x)=x^2-1$ and $h_3(x)=x^3-3x$. Hence

$$
\boxed{H_1(B_t,t)=B_t,\qquad H_2(B_t,t)=B_t^2-t,\qquad H_3(B_t,t)=B_t^3-3tB_t.}
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
