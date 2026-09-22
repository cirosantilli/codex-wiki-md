<h1 id="5/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

At $\Omega=\kappa$, the inverse-transform denominator is $-(\omega-i\kappa)^2$. For $t>0$, its upper-half-plane double-pole [residue](../../../../../../residue.md) is the [derivative](../../../../../../derivative.md) of the exponential:

$$
G(t)=-i\left.\frac{d}{d\omega}e^{i\omega t}\right|_{\omega=i\kappa}
=\boxed{t e^{-\kappa t}}.
$$

It is also the continuous limit of both answers above as $\beta\to0$ or $\eta\to0$. This [critically damped](../../../../../../critical-damping.md) response tends to zero with a linear factor multiplying the exponential.

In all three cases, for $t<0$ close the [contour](../../../../../../complex-integration-contour.md) in the lower half-plane, where $e^{i\omega t}$ decays. There are no [poles](../../../../../../pole.md) inside, so

$$
\boxed{G(t)=0\quad(t<0)}.
$$

At $t=0$ its continuous value is zero and $G'(0^+)=1$, producing the unit [derivative](../../../../../../derivative.md) jump required by $(D_t^2+2\kappa D_t+\Omega^2)G=\delta(t)$. Thus all three formulas are causal [Green's functions](../../../../../../green-s-function-split.md) and all decay to zero at late times.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [5](../../../5.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
