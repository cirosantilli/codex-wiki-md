<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use a mostly-plus target [Minkowski spacetime](../../../../../minkowski-spacetime.md) metric and restore the [string tension](../../../../../string-tension.md) by $T=(2\pi\alpha')^{-1}$. After [Wick rotation](../../../../../wick-rotation.md), the [Polyakov action](../../../../../polyakov-action.md) on a [Riemann surface](../../../../../riemann-surfaces.md) is

$$
S_E=\frac1{4\pi\alpha'}\int_\Sigma\sqrt h\,h^{\mu\nu}\partial_\mu X^a\partial_\nu X_a.
$$

The [Polyakov path integral](../../../../../polyakov-path-integral.md) integrates over embeddings and [worldsheet metrics](../../../../../worldsheet-metric.md), dividing by [worldsheet diffeomorphisms](../../../../../worldsheet-diffeomorphism.md) and [Weyl transformations](../../../../../weyl-transformation.md). For a consistent flat [bosonic string theory](../../../../../bosonic-string-theory.md), take the [critical dimension of the bosonic string](../../../../../critical-dimension-of-string-theory.md) $d=26$. [Conformal gauge](../../../../../conformal-gauge.md) turns the embedding fields into free scalars; its [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) is represented by the [bc system](../../../../../bc-system.md). The remaining integrations are over [worldsheet moduli](../../../../../worldsheet-moduli.md) and external insertion points.

A [tachyon vertex operator](../../../../../tachyon-vertex-operator.md) is

$$
V_k(z,\bar z)={}:e^{ik\cdot X(z,\bar z)}:.
$$

The [worldsheet Green function](../../../../../worldsheet-green-function.md) is $\langle X^a(z)X^b(w)\rangle=-(\alpha'/2)\eta^{ab}\log|z-w|^2$. The [operator product expansion](../../../../../operator-product-expansion.md) with the [holomorphic stress-energy tensor](../../../../../holomorphic-stress-energy-tensor.md) gives [conformal weights](../../../../../conformal-weight.md) $(\alpha' k^2/4,\alpha' k^2/4)$. An [integrated string vertex operator](../../../../../integrated-string-vertex-operator.md) must have weights $(1,1)$, so the [mass-shell condition](../../../../../string-mass-shell-condition.md) is $k^2=4/\alpha'$, or tachyonic [mass](../../../../../mass.md) parameter $m^2=-4/\alpha'$.

At lowest order in the [string coupling](../../../../../string-coupling.md), the [worldsheet](../../../../../worldsheet.md) is a [Riemann sphere](../../../../../riemann-sphere.md). For four external states, three insertion points can be fixed by a [Möbius transformation](../../../../../mobius-transformation.md). In the [worldsheet ghost field](../../../../../worldsheet-ghost-field.md) description these three vertices carry $c\bar c$, while the fourth is integrated. The [three-point worldsheet ghost correlator](../../../../../three-point-worldsheet-ghost-correlator.md) gives the squared product of the three fixed-point separations, precisely the [sphere gauge fixing for four string vertices](../../../../../sphere-gauge-fixing-for-four-string-vertices.md) factor. Thus fixing three points is a gauge choice, rather than deleting three integrations without their Jacobian.

The [integral](../../../../../integral.md) over the constant embedding [worldsheet zero mode](../../../../../worldsheet-zero-mode.md) gives $(2\pi)^d\delta^{(d)}(\sum_i k_i)$. The remaining [Gaussian integral](../../../../../gaussian-integral.md), using [normal ordering](../../../../../normal-ordering.md) to remove self-contractions, gives the [Koba-Nielsen factor](../../../../../koba-nielsen-factor.md)

$$
\left\langle\prod_{i=1}^4 V_{k_i}(z_i,\bar z_i)\right\rangle
\ \propto\
\delta^{(d)}\!\left(\sum_i k_i\right)
\prod_{i<j}|z_i-z_j|^{\alpha' k_i\cdot k_j}.
$$

Set $(z_1,z_2,z_3,z_4)=(0,z,1,\infty)$; the vertex at infinity is defined with its conformal-weight factor. Let all momenta be incoming and define

$$
s=-(k_1+k_2)^2,\qquad t=-(k_2+k_3)^2,\qquad u=-(k_1+k_3)^2.
$$

The [mass-shell condition](../../../../../string-mass-shell-condition.md) and [momentum conservation](../../../../../momentum-conservation.md) imply $s+t+u=-16/\alpha'$. Since $\alpha'k_1\cdot k_2=-4-\alpha's/2$ and similarly for the pair $(2,3)$, the [sphere tachyon position integral](../../../../../sphere-tachyon-position-integral.md) becomes

$$
\mathcal A_4^{(0)}
=\mathcal N g_s^2(2\pi)^d\delta^{(d)}\!\left(\sum_i k_i\right)
\int_{\mathbb C}d^2z\,|z|^{-4-\alpha's/2}|1-z|^{-4-\alpha't/2}.
$$

Here $\mathcal N$ depends on the normalization of external [string vertex operators](../../../../../string-vertex-operator.md); it does not affect the kinematic dependence.

To evaluate the remaining [worldsheet modulus](../../../../../worldsheet-moduli.md), put $a=-1-\alpha's/4$ and $b=-1-\alpha't/4$. The [complex beta integral](../../../../../complex-beta-integral.md) is

$$
\int_{\mathbb C}d^2z\,|z|^{2a-2}|1-z|^{2b-2}
=\pi\frac{\Gamma(a)\Gamma(b)\Gamma(1-a-b)}
{\Gamma(1-a)\Gamma(1-b)\Gamma(a+b)}.
$$

For example, this identity follows by writing the two powers as Schwinger-parameter [Gamma integrals](../../../../../gamma-integral.md), doing the two-dimensional [Gaussian integral](../../../../../gaussian-integral.md), and changing the two positive parameters to their sum and ratio. The [complex beta integral](../../../../../complex-beta-integral.md) first holds for $\operatorname{Re}a,\operatorname{Re}b>0$ and $\operatorname{Re}(a+b)<1$; the scattering result is its [analytic continuation](../../../../../analytic-continuation.md). The third gamma-function argument is $1-a-b=-1-\alpha'u/4$. Absorbing $\pi$ into $\mathcal N$, the result is the **tree-level four-tachyon amplitude**, the [Virasoro–Shapiro amplitude](../../../../../virasoro-shapiro-amplitude.md):

$$
\boxed{\mathcal A_4^{(0)}
=\mathcal C g_s^2(2\pi)^d\delta^{(d)}\!\left(\sum_i k_i\right)
\prod_{q\in\{s,t,u\}}\frac{\Gamma(-1-\alpha'q/4)}{\Gamma(2+\alpha'q/4)}.}
$$

It is symmetric in the three [Mandelstam variables](../../../../../mandelstam-variables.md) and has generic poles at $q=4(N-1)/\alpha'$, matching the [bosonic string mass spectrum](../../../../../bosonic-string-mass-spectrum.md). The formula is the leading term of [string perturbation theory](../../../../../string-perturbation-theory.md). Higher orders are constructed by the same [Polyakov path integral](../../../../../polyakov-path-integral.md) prescription on higher-[genus](../../../../../genus-of-a-surface.md) [worldsheets](../../../../../worldsheet.md), with four marked points and the corresponding ghost and [worldsheet moduli](../../../../../worldsheet-moduli.md) measure; genus $g$ has coupling power $g_s^{2g+2}$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
