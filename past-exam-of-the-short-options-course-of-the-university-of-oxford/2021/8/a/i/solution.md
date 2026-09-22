<h1 id="8/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Differentiate the [worldline](../../../../../world-line.md) with respect to $\theta$:

$$
\frac{dt}{d\theta}=\sqrt2T\cos\theta>0,\qquad \frac{dx}{d\theta}=-\sqrt2cT\kappa\sin\theta,\qquad\frac1c\frac{dx}{dt}=-\kappa\tan\theta.
$$

Since $|\tan\theta|\le1$ and $0<\kappa<1$, this is a future-directed [timelike curve](../../../../../timelike-curve.md). The [proper time](../../../../../proper-time.md) element satisfies $c^2d\tau^2=c^2dt^2-dx^2$, hence

$$
\frac{d\tau}{d\theta}=\sqrt2T\sqrt{\cos^2\theta-\kappa^2\sin^2\theta}.
$$

Alice's total [proper time](../../../../../proper-time.md) is therefore

$$
\boxed{\tau_A=2\sqrt2T\int_0^{\pi/4}\sqrt{1-(1+\kappa^2)\sin^2\theta}\,d\theta.}
$$

This definite integral is an exact answer; it is an [elliptic integral of the second kind](../../../../../elliptic-integral-of-the-second-kind.md). In notation $E(\alpha\mid m)=\int_0^\alpha\sqrt{1-m\sin^2u}\,du$, it is $2\sqrt2T E(\pi/4\mid1+\kappa^2)$. Although this parameter exceeds one, the integrand is real on the stated interval because its minimum squared value is $(1-\kappa^2)/2>0$.

The endpoint events have $(t,x)=(0,0)$ and $(2T,0)$. Sam stays at $x=0$ in his [inertial frame](../../../../../inertial-frame.md), so his elapsed [proper time](../../../../../proper-time.md) is $2T$. For $\kappa>0$, the integrand is strictly less than $\cos\theta$ except at $\theta=0$, and $\tau_A<2T$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
