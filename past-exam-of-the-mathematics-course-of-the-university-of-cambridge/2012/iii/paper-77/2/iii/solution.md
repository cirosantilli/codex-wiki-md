<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take $\beta\ge0$ without loss of generality, since its definition fixes only $\beta^2$. With $r_s=\beta^2\tau$, the steady-branch minimum expands as $r_{\rm min}=1+2\beta\tau+O(\tau^2)$. For fixed positive $\sigma$, the source's supplied approximation therefore gives

$$
r^{(0)}_{\rm supplied}-r_{\rm min}=\tau\left(\delta+\frac{\beta^2}{\delta}-2\beta\right)+O(\tau^2)=\frac{\tau}{\delta}(\beta-\delta)^2+O(\tau^2)\ge0\quad\text{to the retained order}.
$$

Thus **the requested inequality follows from the supplied approximation**, with equality at first order when $\beta=\delta$. If negative $\beta$ is retained, replace it by $|\beta|$ throughout.

There is an independent source-consistency issue with calling that supplied expression the oscillatory threshold of the displayed model. Linearizing about conduction, the $c,e$ modes decay separately and the $a,b,d$ characteristic polynomial is

$$
(\lambda+\sigma)(\lambda+1)(\lambda+\tau)-\sigma r(\lambda+\tau)+\sigma r_s(\lambda+1)=0.
$$

Writing it as $\lambda^3+A\lambda^2+B\lambda+C$, a nonzero imaginary pair requires $C=AB$ and $B>0$, by the [Routh-Hurwitz stability criterion](../../../../../../routh-hurwitz-stability-criterion.md). Direct algebra gives the [oscillatory threshold of a thermosolutal Lorenz model](../../../../../../oscillatory-threshold-of-a-thermosolutal-lorenz-model.md)

$$
r_H=1+\frac{\tau(\sigma+1+\tau)}{\sigma}+\frac{\sigma+\tau}{\sigma+1}r_s,\qquad \omega_H^2=\frac{\sigma}{\sigma+1}r_s(1-\tau)-\tau^2.
$$

Consequently, with $\delta=\sigma/(1+\sigma)$,

$$
\boxed{r_H=1+\frac{\tau}{\delta}+\beta^2\tau\delta+O(\tau^2).}
$$

The two factors of $\delta$ in the supplied threshold are interchanged. For example $\sigma=1$, $\beta=2$, $\tau=10^{-3}$ gives a genuine marginal imaginary pair at $r_H=1.004003$, whereas the supplied first-order expression gives $1.0085$. The intended comparison remains true after correction:

$$
\boxed{r_H-r_{\rm min}=\frac{\tau}{\delta}(\beta\delta-1)^2+O(\tau^2)\ge0\text{ to first order}.}
$$

This comparison applies to a physical [Hopf bifurcation](../../../../../../hopf-bifurcation.md) when $\omega_H^2>0$ and to an interior steady fold when $a_*^2>0$. For fixed nonzero $\beta$ and fixed $\sigma>0$, both conditions hold for sufficiently small positive $\tau$. At a vanishing squared difference, neglected terms must be examined before drawing a higher-order conclusion.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Section I](../../section-i.md)
4. [Paper 77](../../../paper-77-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
