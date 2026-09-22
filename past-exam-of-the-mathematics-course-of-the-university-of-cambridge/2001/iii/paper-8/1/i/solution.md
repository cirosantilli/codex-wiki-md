<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [polar coordinates](../../../../../../polar-coordinates.md) $x=r\cos\theta$, $y=r\sin\theta$. Away from the crossing, the [lemniscate of Bernoulli](../../../../../../lemniscate-of-bernoulli.md) has $r^2=\cos2\theta$. An explicit parametrization of its four quarter-arcs is

$$
\boxed{x=\pm t\sqrt{\frac{1+t^2}{2}},\qquad y=\pm t\sqrt{\frac{1-t^2}{2}},\qquad 0\leq t\leq1},
$$

where the two signs are independent. Indeed $x^2+y^2=t^2$ and $x^2-y^2=t^4$. The four arcs meet at the origin and at the two lobe endpoints, covering the entire curve.

For the upper-right quarter, take $0\leq\theta\leq\pi/4$, $r=\sqrt{\cos2\theta}$. Differentiating gives $dr/d\theta=-\sin2\theta/r$. Thus the [arc length](../../../../../../arc-length.md) element satisfies

$$
\left(\frac{ds}{d\theta}\right)^2=r^2+\left(\frac{dr}{d\theta}\right)^2
=\frac{\cos^22\theta+\sin^22\theta}{\cos2\theta}=\frac1{r^2}.
$$

Set $t=r$, which decreases from one to zero. Since $|dt/d\theta|=\sqrt{1-t^4}/t$, it follows that $ds=|dt|/\sqrt{1-t^4}$. All four quarter-arcs have the same length, so

$$
\boxed{L=4\int_0^1\frac{dt}{\sqrt{1-t^4}}}.
$$

The endpoint singularity is proportional to $(1-t)^{-1/2}$ and is integrable. This is the geometric origin of the [lemniscatic integral](../../../../../../lemniscatic-integral.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
