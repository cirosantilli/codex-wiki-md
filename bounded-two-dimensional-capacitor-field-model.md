# Bounded two-dimensional capacitor field model

↑ **Parent:** [Fringing field of a capacitor](fringing-field-of-a-capacitor.md)

The diagrams solve an explicitly bounded [Dirichlet problem](dirichlet-problem.md) in a uniform charge-free medium of constant [permittivity](permittivity-split.md). Take a width scale $W=1$ and terminal [electric potential difference](electric-potential-difference.md) $V=1$. Two zero-thickness ideal plate segments occupy $|x|\leq W/2$ at $y=\pm d/2$, with [electric potentials](electric-potential.md) $\pm V/2$. Fix $\phi=0$ on the entire rectangle $x=\pm2W$, $y=\pm1.5W$. This boundary is an additional enclosing [equipotential](equipotential.md), rather than a condition at infinity. The model is invariant along the omitted third direction. The connection between the [electric potential](electric-potential.md), its [gradient](gradient.md), and the charge-free [Laplace equation](laplace-equation.md) follows from [electrostatics](electrostatics-split.md).[II.6–1, equations (6.3)–(6.6)](the-feynman-lectures-on-physics-volume-ii-by-richard-feynman-and-others.md)

On a square mesh of spacing $h=W/160$, the [finite difference method](finite-difference-method.md) imposes

$$
\phi_{i,j}=\frac14\left(\phi_{i+1,j}+\phi_{i-1,j}+\phi_{i,j+1}+\phi_{i,j-1}\right)
$$

at free nodes, while plate and outer nodes retain their prescribed [electric potentials](electric-potential.md). There are $641\times481$ nodes. Each plotted gap aligns exactly with the mesh; the smallest gap has 16 mesh intervals. The generators solve the resulting [linear system](system-of-linear-equations.md) by the [Conjugate gradient method](conjugate-gradient-method.md), stopping when the maximum dimensionless five-point residual is below $2\times10^{-10}$, and use [central finite differences](central-finite-difference.md) to approximate $\mathbf E=-\nabla\phi$ away from plate nodes.

The [discrete maximum principle](discrete-maximum-principle.md) keeps the computed [electric potential](electric-potential.md) between $-V/2$ and $+V/2$. Reflection checks require evenness in $x$ and oddness in $y$; halving $h$ tests discretization effects, while enlarging the outer rectangle tests sensitivity to its artificial [boundary conditions](boundary-condition.md). These are different checks: a small residual only establishes that the discrete equations were solved. Differentiating near zero-thickness endpoints is especially sensitive to the mesh, so the plots do not report a converged edge peak. No total [electric charge](electric-charge-split.md), exact open-domain three-dimensional [capacitance](capacitance.md), or measured material property is extracted from this model.

For a bounded numerical check, compare $h=W/80$ with the plotted $h=W/160$ at midplane positions $x/W=0,0.25,0.40,0.50,0.60,0.80$. At $d/W=0.10$, the largest change in $-E_y d/V$ is approximately $0.0265$, at $x/W=0.50$; the other five sampled changes are below $0.00472$. At $d/W=0.25$, moving the outer rectangle from $\pm2W\times\pm1.5W$ to $\pm3W\times\pm2W$ while retaining $h=W/80$ changes these samples by at most approximately $0.00622$. These calculated sensitivities support the qualitative comparison and expose its limits; they are not experimental uncertainties or evidence that the artificial boundary has converged to infinity.

## ↑ Ancestors (7)

1. [Fringing field of a capacitor](fringing-field-of-a-capacitor.md)
2. [Parallel-plate capacitor](parallel-plate-capacitor.md)
3. [Capacitor](capacitor.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Capacitor gap aspect ratio](capacitor-gap-aspect-ratio.md)
- [Fringing field of a capacitor](fringing-field-of-a-capacitor.md)
