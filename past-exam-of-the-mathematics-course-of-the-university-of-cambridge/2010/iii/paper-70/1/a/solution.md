<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a [Fourier transform](../../../../../../fourier-transform.md) parallel to the boundary. Splitting its traces into right- and left-supported parts gives [Half-range Fourier transforms](../../../../../../half-range-fourier-transform.md) $F_+$ and $F_-$, analytic respectively above and below a common inversion contour. A small positive imaginary part of the [wavenumber](../../../../../../wavenumber.md) implements the [limiting absorption principle](../../../../../../limiting-absorption-principle.md) and separates the incident [poles](../../../../../../pole.md) and outgoing [branch points](../../../../../../branch-point.md). Solve the transformed differential equation normal to the boundary using its outgoing or decaying solution. The boundary conditions then yield a [Wiener-Hopf equation](../../../../../../wiener-hopf-equation.md) of the form

$$
K(\alpha)F_+(\alpha)=F_-(\alpha)+H(\alpha).
$$

Factor its [Wiener-Hopf kernel](../../../../../../wiener-hopf-kernel.md) as $K=K_+K_-$, with each factor analytic and nonzero in its designated half-plane. Divide by $K_-$ and split $H/K_-=H_++H_-$, allocating [poles](../../../../../../pole.md) according to the incident-wave prescription. Then

$$
K_+F_+-H_+=F_-/K_-+H_-.
$$

The two sides continue to a common [entire function](../../../../../../entire-function.md). Their growth at infinity, inherited from the field's edge behavior, determines that [function](../../../../../../function-split.md), usually a constant or a [polynomial](../../../../../../polynomial-split.md); in a decaying case it is zero. Solve for the unknown transforms and apply [Fourier inversion](../../../../../../fourier-inversion-theorem.md), preserving the outgoing contour prescription.

The principal analytic results used are as follows. The [Paley–Wiener theorem](../../../../../../paley-wiener-theorem.md) and its half-line Laplace-transform version relate support on a half-line to holomorphy in a half-plane, with growth or square-integrability bounds. The [Cauchy integral formula](../../../../../../cauchy-integral-formula.md) and [Sokhotski–Plemelj theorem](../../../../../../sokhotski-plemelj-theorem.md) provide additive splitting: a Cauchy [integral](../../../../../../integral.md) of a sufficiently decaying jump has upper and lower boundary values with that prescribed difference. Applying the same construction to a continuous logarithm of a nonvanishing scalar [Wiener-Hopf kernel](../../../../../../wiener-hopf-kernel.md) gives [Wiener-Hopf factorization](../../../../../../wiener-hopf-factorization.md) when its [winding number](../../../../../../winding-number.md) is zero; a nonzero index requires an explicit index factor. The [identity theorem](../../../../../../identity-theorem.md) gives [analytic continuation](../../../../../../analytic-continuation.md) across the common strip. Finally [Liouville's theorem](../../../../../../liouville-theorem.md) makes a bounded [entire function](../../../../../../entire-function.md) constant; its polynomial-growth extension bounds the possible degree. The physical edge and [radiation conditions](../../../../../../radiation-condition.md) select the remaining constants. Zeros, [branch cuts](../../../../../../branch-cut.md), nonzero index and insufficient decay must be accounted for rather than discarded during splitting.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
