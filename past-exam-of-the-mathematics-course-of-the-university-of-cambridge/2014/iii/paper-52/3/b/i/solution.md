<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $A=r^2+a^2$, $s=\sin\theta$, $\Sigma=A-a^2s^2$, and $\Delta=A-2Mr$. Use [ingoing Kerr coordinates](../../../../../../../ingoing-kerr-coordinates.md), so $dt=dv-A\,dr/\Delta$ and $d\phi=d\chi-a\,dr/\Delta$. To see the cancellations without expanding every term, write the [Kerr metric](../../../../../../../kerr-metric.md) in the equivalent form

$$
ds^2=-\frac\Delta\Sigma(dt-a s^2d\phi)^2+\frac\Sigma\Delta dr^2+\Sigma d\theta^2+\frac{s^2}\Sigma(A\,d\phi-a\,dt)^2.
$$

The combinations become

$$
dt-a s^2d\phi=dv-a s^2d\chi-\frac\Sigma\Delta dr,\qquad A\,d\phi-a\,dt=A\,d\chi-a\,dv.
$$

The first square contributes $-\Sigma dr^2/\Delta$, cancelling the explicit radial term. Expanding the remaining terms gives

$$
\boxed{\begin{aligned}
ds^2={}&-\left(1-\frac{2Mr}\Sigma\right)dv^2+2\,dv\,dr-\frac{4Mar s^2}\Sigma\,dv\,d\chi-2a s^2\,dr\,d\chi\\
&+\Sigma\,d\theta^2+\left(A+\frac{2Ma^2r s^2}\Sigma\right)s^2d\chi^2.
\end{aligned}}
$$

There is no denominator $\Delta$ in this [Lorentzian metric](../../../../../../../lorentzian-metric.md). At the outer horizon $r_+=M+\sqrt{M^2-a^2}$, $\Sigma>0$ and the components are smooth. The determinant is $-\Sigma^2\sin^2\theta$, so away from the usual polar-coordinate degeneracy the metric is nondegenerate and extends across $r_+$. The axis can be covered by regular angular charts. Thus the [Boyer-Lindquist coordinates](../../../../../../../boyer-lindquist-coordinates.md) are singular there, while the [ingoing Kerr coordinates](../../../../../../../ingoing-kerr-coordinates.md) are regular at the future horizon.

For physical nonextremality the invariant parameter condition is $M>|a|$, $M>0$. The printed $M>a$ is sufficient when the rotation orientation has been chosen so that $a\geq0$; without that convention it needs the absolute value.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 52](../../../../paper-52-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
