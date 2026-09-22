<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A [Taylor expansion](../../../../../../taylor-expansion.md) of the tangential [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) gives $u_{2x}(0)=-\sin\xi\,\partial_yu_{1x}(0)$. Since $f''(0)=-s$,

$$
\langle u_{2x}(0)\rangle=s\langle\sin^2\xi\rangle=s/2.
$$

For [matrix-relative Brinkman velocity](../../../../../../matrix-relative-brinkman-velocity.md), the mean second-order tangential flow is

$$
\overline u_{2x}(y)=\mathcal U_2+C e^{-Ay}.
$$

The mean tangential traction has no first-order geometric remainder: at the surface $\partial_y\sigma_{xy,1}=s(s+1)\sin\xi$ and $\sigma_{xx,1}=s(s+1)\cos\xi$, so the mean displaced-boundary and tilted-normal corrections cancel. Thus the [force-free](../../../../../../force-free.md) condition gives $\overline u_{2x}'(0)=0$, hence $C=0$. In the $A=0$ limit boundedness likewise excludes mean shear. The [swimming speed of a Brinkman sheet](../../../../../../swimming-speed-of-a-brinkman-sheet.md) is therefore

$$
\boxed{\mathcal U=\frac{\epsilon^2}{2}\sqrt{1+A^2}+O(\epsilon^4),\qquad
U=\frac{b^2k\omega}{2}\sqrt{1+(\alpha/k)^2}+O\!\left(\frac\omega k\epsilon^4\right).}
$$

It is larger than the simple-fluid speed by $\sqrt{1+(α/k)^2}$ for fixed waveform and frequency. The matrix offers a reaction structure for the transverse stroke and more strongly confines the induced motion; it acts as a footing against which the wave pushes. This is a prescribed-stroke comparison, not a guarantee at fixed motor power. The small-amplitude expansion is at fixed $A$; a large-$A$ use also needs $\epsilon s\ll1$ to control variation across the displaced boundary.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
