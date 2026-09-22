<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose the internal transverse force $S(x,t)$ so that the net internal transverse [force](../../../../../../force.md) on a slice is $[S(x+dx,t)-S(x,t)]$. Its [linear momentum](../../../../../../momentum.md) balance is then

$$
m_b(x)h_{tt}\,dx=S_x\,dx+F_y\,dx.
$$

The coordinate $x$ labels body slices, so their lateral material acceleration is $h_{tt}$; the fluid transport operator $\mathcal D$ must not be substituted for this body acceleration.

Let $G$ be the total internal [bending moment](../../../../../../bending-moment.md), including both passive elastic and active muscular contributions. With the compatible moment orientation, the net couple on the slice is $(G_x-S)\,dx$. The cross-sectional rotary inertia is smaller than the translational inertia by the square of the transverse-to-longitudinal length ratio, and is neglected in this slender-beam approximation. Slice [angular momentum](../../../../../../angular-momentum.md) balance therefore gives $S=G_x$. Eliminating $S$ from the slice [linear momentum](../../../../../../momentum.md) balance proves

$$
\boxed{G_{xx}=m_bh_{tt}-F_y.}
$$

This equation is the balance law for an [active bending beam for a swimming fish](../../../../../../active-bending-beam-for-a-swimming-fish.md); a constitutive relation for the passive [bending moment](../../../../../../bending-moment.md) or the muscle actuation is not needed to derive it. With the force-on-body convention established above it becomes

$$
G_{xx}=m_bh_{tt}+\mathcal D(m\mathcal Dh).
$$

As a check, constant $m$ and rigid lateral acceleration give the effective inertia $m_b+m$. Combining the printed positive force in part (i) with the minus sign in the beam equation would instead give $m_b-m$. That is the same sign defect, rather than a negative hydrodynamic [added mass](../../../../../../added-mass.md). If the positive quantity in part (i) is called $F_y$ as a force on the fluid, the beam equation must contain $+F_y$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
