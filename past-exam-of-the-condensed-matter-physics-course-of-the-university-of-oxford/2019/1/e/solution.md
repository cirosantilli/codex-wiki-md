<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

In cubic coordinates write $\mathbf G=(2\pi/a)(h,k,l)$. The [face-centred cubic selection rule](../../../../face-centred-cubic-selection-rule.md) allows integer triples only when $h,k,l$ are all even or all odd. One way to derive it is to sum the four conventional-cell lattice positions:

$$
F_{\mathrm{fcc}}=1+(-1)^{h+k}+(-1)^{h+l}+(-1)^{k+l}.
$$

This vanishes for mixed parity and equals four otherwise. The two-atom diamond [atomic basis](../../../../atomic-basis-of-a-crystal.md) adds the factor

$$
F_{\mathrm{basis}}=b(\mathbf G)\left[1+e^{i\pi(h+k+l)/2}\right].
$$

For all-odd indices this is nonzero. For all-even indices it vanishes when $h+k+l=2\pmod4$ and survives when the sum is divisible by four: this is [diamond-basis diffraction extinction](../../../../diamond-basis-diffraction-extinction.md).

Exclude the forward beam $000$ and order the remaining families by $h^2+k^2+l^2$. The first is $111$, with squared length three. The candidate $200$, with squared length four, is extinguished by the diamond [atomic basis](../../../../atomic-basis-of-a-crystal.md). The next allowed family is $220$, with squared length eight. Thus

$$
\boxed{|\mathbf G_1|=\frac{2\pi\sqrt3}{a}\quad(111),\qquad|\mathbf G_2|=\frac{2\pi\sqrt8}{a}=\frac{4\pi\sqrt2}{a}\quad(220).}
$$

For fixed incident [wavelength](../../../../wavelength.md), $|\mathbf G|=2k\sin\theta$ increases with scattering angle, so these are the two lowest-angle powder rings. The two atoms are counted per primitive cell; a conventional silicon cube contains four lattice points and eight atoms.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
