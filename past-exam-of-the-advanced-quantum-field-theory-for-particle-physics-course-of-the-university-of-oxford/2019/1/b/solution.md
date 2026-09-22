<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the one-loop [renormalization-group beta function](../../../../beta-function-physics.md), write $t=\log\mu$. Separating variables gives

$$
\int_{\alpha_i}^{\alpha_f}\frac{d\alpha}{\alpha^2}=b_0\int_{\log\mu_i}^{\log\mu_f}dt,
\qquad
\boxed{\alpha(\mu_f)=\frac{\alpha(\mu_i)}{1-b_0\alpha(\mu_i)\log(\mu_f/\mu_i)}.}
$$

This expression resums the leading logarithms of the one-loop [running coupling](../../../../running-coupling.md), while omitting higher-order terms in the [renormalization-group beta function](../../../../beta-function-physics.md). Assume a positive initial coupling.

For $b_0<0$, increasing the [renormalization scale](../../../../renormalization-scale.md) decreases the [running coupling](../../../../running-coupling.md); the zero-coupling [renormalization-group fixed point](../../../../renormalization-group-fixed-point.md) is attractive in the ultraviolet. This is [asymptotic freedom](../../../../asymptotic-freedom.md). Toward lower scales the one-loop expression has a formal pole at $\mu_i\exp[1/(b_0\alpha_i)]<\mu_i$. The strong-coupling neighborhood of that pole lies outside perturbative control. [QCD](../../../../quantum-chromodynamics.md) provides the main example; the minimal [Standard Model](../../../../standard-model-split.md) $SU(2)$ coupling is also [asymptotically free](../../../../asymptotic-freedom.md) at one loop.

For $b_0>0$, the [running coupling](../../../../running-coupling.md) grows with the [renormalization scale](../../../../renormalization-scale.md) and formally diverges at the ultraviolet [Landau pole](../../../../landau-pole.md) $\mu_i\exp[1/(b_0\alpha_i)]>\mu_i$. Toward the infrared it decreases to zero within this approximation. The [Standard Model](../../../../standard-model-split.md) $U(1)$ [weak hypercharge](../../../../hypercharge.md) coupling has this sign, as does [QED](../../../../quantum-electrodynamics.md) in a fixed charged-particle regime. A perturbative [Landau pole](../../../../landau-pole.md) marks failure of the approximation, rather than proving that the exact theory has that divergence.

For $b_0=0$, the [running coupling](../../../../running-coupling.md) is constant at this order; higher-loop terms decide whether it runs. Vanishing of the leading coefficient alone does not establish exact scale invariance.

For a concrete common convention, define $\alpha_i=g_i^2/(4\pi)$ with $g_Y$ in its usual, non-unified [weak hypercharge](../../../../hypercharge.md) normalization. In the minimal [Standard Model](../../../../standard-model-split.md) with three generations and one Higgs doublet, above its particle thresholds,

$$
\frac{d\alpha_i}{d\log\mu}=\frac{b_i}{2\pi}\alpha_i^2,\qquad
(b_Y,b_2,b_3)=\left(\frac{41}{6},-\frac{19}{6},-7\right).
$$

Thus the question's $b_0$ is $b_i/(2\pi)$, with the sign regimes just described. Crossing a [mass](../../../../mass.md) threshold changes the active field content and requires the appropriate piecewise [renormalization-group beta function](../../../../beta-function-physics.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
