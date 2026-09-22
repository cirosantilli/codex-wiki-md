<h1 id="2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Part (ii) represents the process as an [Iterated Itô integral](../../../../../iterated-ito-integral.md):

$$
B_t^3-3tB_t=6I_3(t)=3\int_0^t(B_s^2-s)\,dB_s.
$$

For a centered [normal random variable](../../../../../gaussian-random-variable.md) $B_s$ of [variance](../../../../../variance-split.md) $s$,

$$
\mathbb E(B_s^2-s)^2=3s^2-2s^2+s^2=2s^2.
$$

Consequently, for every finite $T$,

$$
\mathbb E\int_0^T(B_s^2-s)^2ds=\frac{2T^3}{3}<\infty.
$$

The [Itô integral](../../../../../ito-integral.md) of this [square-integrable stochastic integrand](../../../../../square-integrable-stochastic-integrand.md) is a true [square-integrable](../../../../../square-integrable-function.md) [martingale](../../../../../martingale-split.md) on $[0,T]$. Since $T$ is arbitrary,

$$
\boxed{B_t^3-3tB_t\text{ is a martingale},\qquad
\mathbb E(B_t^3-3tB_t)^2=6t^3.}
$$

The last identity is the [Itô isometry](../../../../../ito-isometry.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../../split.md)
6. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
