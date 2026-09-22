<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [mobility correction from a fixed distant sphere](../../../../../../mobility-correction-from-a-fixed-distant-sphere.md) gives

$$
\dot Y=-\frac{27Va^2}{16}\frac{XY}{(X^2+Y^2)^2},\qquad\dot X=V\left[1+O(a^2/R^2)\right].
$$

Taking their ratio and keeping the first nonzero transverse correction yields

$$
\boxed{\frac{dY}{dX}=-\frac{27a^2}{16}\frac{XY}{R^4}}
$$

to the stated leading order. Set $b=Y_\infty\gg a$. The deflection is $O(a^2/b)$, so replacing $Y$ by $b$ on the right introduces only higher-order errors. Integrating from $X=-\infty$ gives

$$
Y(X)-b=\frac{27a^2b}{32(X^2+b^2)}+O(a^4/b^3).
$$

The maximum occurs at $X=0$, and the [deflection and spin in a distant sphere encounter](../../../../../../deflection-and-spin-in-a-distant-sphere-encounter.md) are

$$
\boxed{\max(Y-Y_\infty)=\frac{27a^2}{32Y_\infty}+O(a^4/Y_\infty^3).}
$$

For the rotation, use $dt=dX/V$ and $Y=b$ to leading order in the [angular velocity](../../../../../../angular-velocity.md) from part (b). Its signed angle about the positive $z$ axis is

$$
\Delta\vartheta=-\frac{9a^2b}{16}\int_{-\infty}^{\infty}\frac{dX}{(X^2+b^2)^2}+O(a^4/b^4)=\boxed{-\frac{9\pi a^2}{32Y_\infty^2}+O(a^4/Y_\infty^4).}
$$

Thus the rotation is clockwise when viewed from positive $z$, with the magnitude of the displayed leading term.

The deflection tends back to zero downstream: **$Y(+\infty)=Y_\infty$**. More generally, [kinematic reversibility of Stokes flow](../../../../../../kinematic-reversibility-of-stokes-flow.md) combined with reflection in the plane $X=0$ makes a passing trajectory fore-aft symmetric. One can see this without using the distant-sphere approximation: the relevant translational [hydrodynamic mobility matrix](../../../../../../hydrodynamic-mobility-matrix.md) has the form $m_\perp(R)I+[m_\parallel(R)-m_\perp(R)]\mathbf n\mathbf n$. Hence $\dot X$ is even in $X$ and $\dot Y$ is odd in $X$. Uniqueness of the trajectory through $X=0$ then gives $Y(X)=Y(-X)$.

For $Y_\infty=a/100$, the numerical deflection and spin approximations above are invalid: the encounter enters a narrow gap and requires [lubrication theory](../../../../../../lubrication-theory.md). However, **the same return to the incoming offset holds for an ideal passing encounter of perfectly smooth [spheres](../../../../../../sphere.md) in [Stokes flow](../../../../../../stokes-flow-split.md)**. [Lubrication resistance](../../../../../../lubrication-resistance.md) prevents finite-time contact under a bounded [force](../../../../../../force.md), and does not itself destroy [kinematic reversibility of Stokes flow](../../../../../../kinematic-reversibility-of-stokes-flow.md). Contact, surface roughness or nonhydrodynamic [forces](../../../../../../force.md) could change that conclusion; they are additional physics, not part of the ideal model. This distinction is the [fore-aft symmetry of a sedimenting-sphere encounter](../../../../../../fore-aft-symmetry-of-a-sedimenting-sphere-encounter.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
