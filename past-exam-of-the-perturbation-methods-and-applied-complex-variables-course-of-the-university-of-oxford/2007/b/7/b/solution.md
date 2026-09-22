<h1 id="b/7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
q_j=\sqrt{\kappa_j^2+i\epsilon}\quad(j=0,1)
$$

be the root with positive real and positive imaginary parts. More explicitly, with $r_j=\sqrt{\kappa_j^4+\epsilon^2}$,

$$
q_j=\sqrt{\frac{r_j+\kappa_j^2}{2}}+
i\sqrt{\frac{r_j-\kappa_j^2}{2}}.
$$

Decay at each infinity and [continuity](../../../../../continuous-function.md) at zero force $y=Ae^{-iq_0x}$ for $x<0$ and $y=Ae^{iq_1x}$ for $x>0$. The [derivative](../../../../../derivative.md) jump is $i(q_1+q_0)A=1$, so

$$
\boxed{y(x)=\frac1{i(q_0+q_1)}
\begin{cases}e^{-iq_0x},&x<0,\\e^{iq_1x},&x>0.\end{cases}}
$$

The two roots lie in the first quadrant, so their sum cannot vanish.

Integrating the [differential equation](../../../../../differential-equation-split.md) twice by parts on each half-line gives

$$
(q_0^2-k^2)\hat y_-=-y'(0-)+iky(0),\qquad
(q_1^2-k^2)\hat y_+=y'(0+)-iky(0).
$$

Their sum is the stated identity with right side one. Equivalently the global distributional equation is $y''+\kappa^2y=\delta_0$, since the [derivative](../../../../../derivative.md) has jump one.

The direct half-transforms are

$$
\hat y_-=\frac{A}{i(k-q_0)},\qquad
\boxed{\hat y_+=-\frac{A}{i(k+q_1)}
=\frac1{(q_0+q_1)(k+q_1)}.}
$$

Here $\hat y_+$ is analytic above its lower-half-plane pole $-q_1$, while $\hat y_-$ is analytic below its upper-half-plane pole $q_0$.

To recover the same result from the transform identity alone, use [Wiener-Hopf factorization](../../../../../wiener-hopf-factorization.md):

$$
\hat y_++\frac{(q_0-k)(q_0+k)}{(q_1-k)(q_1+k)}\hat y_-
=\frac1{(q_1-k)(q_1+k)}.
$$

Multiply by $(q_1+k)/(q_0+k)$. The coefficient of $\hat y_-$ becomes $(q_0-k)/(q_1-k)$, analytic and zero-free in the lower [half-plane](../../../../../half-plane.md), while the coefficient of $\hat y_+$ is analytic and zero-free in the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md). Split the right side as

$$
\frac1{(q_0+k)(q_1-k)}
=\frac1{q_0+q_1}\left(\frac1{q_0+k}+\frac1{q_1-k}\right).
$$

The first term is analytic above and the second below. Equating the separated [functions](../../../../../function-split.md) and using their decay at infinity fixes the entire remainder to zero, yielding the boxed $\hat y_+$, with the branches fixed before factorization.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
