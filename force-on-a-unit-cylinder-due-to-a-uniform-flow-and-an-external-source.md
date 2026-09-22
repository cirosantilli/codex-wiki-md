# Force on a unit cylinder due to a uniform flow and an external source

↑ **Parent:** [Blasius force theorem](blasius-force-theorem.md)

In a planar [potential flow](potential-flow.md), superpose a positive-$x$ [uniform flow](uniform-flow.md) of speed $U$ and a [line source](line-source.md) of strength $Q=2\pi m$ at the real point $b>1$. Introduce an impermeable unit circular [cylinder](cylinder-geometry.md) with zero [circulation](circulation-physics.md). The [Milne-Thomson circle theorem](milne-thomson-circle-theorem.md) gives the [complex potential of a two-dimensional potential flow](complex-potential-of-a-two-dimensional-potential-flow.md)

$$
w=U(z+z^{-1})+m[\log(z-b)+\log(z-b^{-1})-\log z].
$$

The displayed horizontal [force per unit length](force-per-unit-length.md) acts on the [cylinder](cylinder-geometry.md), and $F_y=0$ by [reflection symmetry](reflection-symmetry.md). To prove it, let $q=w'$ be the [complex velocity](complex-velocity.md). At infinity, $q=U+m/z+O(z^{-2})$, so the sum of all finite [residues](residue.md) of $q^2$ is $2Um$. At the external [pole](pole.md) $b$, write $q=m/(z-b)+H(z)$; then

$$
\operatorname{Res}_{b}q^2=2mH(b),\qquad
H(b)=U-\frac U{b^2}+\frac{m}{b(b^2-1)}.
$$

The [residue theorem](residue-theorem.md) and the counterclockwise [Blasius force theorem](blasius-force-theorem.md) give $F_x-iF_y=2\pi\rho m[H(b)-U]$, proving the formula. With $m>0$ and $U>0$, its sign changes at $b=(m+\sqrt{m^2+4U^2})/(2U)$.

## ↑ Ancestors (7)

1. [Blasius force theorem](blasius-force-theorem.md)
2. [Complex potential of a two-dimensional potential flow](complex-potential-of-a-two-dimensional-potential-flow.md)
3. [Potential flow](potential-flow.md)
4. [Fluid mechanics](fluid-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-fluids-and-waves-course-of-the-university-of-oxford/2021/1/b/ii/solution.md)
