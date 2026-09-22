<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

On a bosonic configuration, the target-space [supersymmetry transformation](../../../../../supersymmetry-transformation.md) changes the fermionic coordinate by $\delta_\epsilon\Theta=\epsilon$, where $\epsilon$ is a background [Killing spinor](../../../../../killing-spinor.md). A [kappa symmetry](../../../../../kappa-symmetry.md) convention is

$$
\delta_\kappa\Theta=(1+\Gamma_\kappa)\kappa,\qquad\Gamma_\kappa^2=1.
$$

The configuration preserves a supersymmetry if this change can be cancelled by a local [kappa symmetry](../../../../../kappa-symmetry.md) transformation. Multiplying $\epsilon+(1+\Gamma_\kappa)\kappa=0$ by $1-\Gamma_\kappa$ proves necessity of

$$
\boxed{\Gamma_\kappa\epsilon=\epsilon.}
$$

Conversely, if this holds, choosing $\kappa=-\epsilon/2$ cancels the variation. Reversing the brane orientation reverses the corresponding [kappa symmetry projector](../../../../../kappa-symmetry-projector.md).

The preserved parameters must solve this equation everywhere on the brane and satisfy the background [Killing spinor](../../../../../killing-spinor.md) equations. Thus the fraction of all thirty-two eleven-dimensional supersymmetries is

$$
\boxed{\frac1{32}\dim_{\mathbb R}\{\epsilon:\epsilon\text{ is a background Killing spinor and }
\Gamma_\kappa(\sigma)\epsilon(X(\sigma))=\epsilon(X(\sigma))\text{ for all }\sigma\}.}
$$

One traceless constant [kappa symmetry projector](../../../../../kappa-symmetry-projector.md) in flat space preserves sixteen parameters. Further independent commuting projectors often halve that number again, but a position-dependent projector requires a common global solution; its pointwise rank alone does not determine the answer. To quote a fraction of the background supersymmetry, divide instead by the number of its [Killing spinors](../../../../../killing-spinor.md).

For the [supermembrane](../../../../../supermembranes.md), let $Z^{\mathcal M}=(X^M,\Theta^\alpha)$ be the embedding in eleven-dimensional [superspace](../../../../../superspace.md). Define the pulled-back [supervielbein](../../../../../supervielbein.md), the [induced worldvolume metric](../../../../../induced-worldvolume-metric.md), and induced [gamma matrices](../../../../../gamma-matrices.md) by

$$
\Pi_i^a=\partial_iZ^{\mathcal M}E_{\mathcal M}{}^a(Z),\qquad
h_{ij}=\Pi_i^a\Pi_j^b\eta_{ab},\qquad \gamma_i=\Pi_i^a\Gamma_a.
$$

For a chosen orientation,

$$
\boxed{\Gamma_\kappa=\frac{\varepsilon^{ijk}}{3!\sqrt{-\det h}}\gamma_{ijk},\qquad
\gamma_{ijk}=\gamma_{[i}\gamma_j\gamma_{k]}.}
$$

The [Clifford algebra](../../../../../clifford-algebra.md) shows that $\Gamma_\kappa^2=1$; in an orthonormal membrane frame this reduces to $(\Gamma_0\Gamma_1\Gamma_2)^2=1$. Its trace is zero, so its two eigenspaces each have real dimension sixteen.

The full [supermembrane action](../../../../../supermembrane-action.md) in an on-shell [eleven-dimensional supergravity](../../../../../eleven-dimensional-supergravity.md) superspace is

$$
\boxed{S=-T_2\int_{\Sigma_3}d^3\sigma\,\sqrt{-\det h}
+qT_2\int_{\Sigma_3}Z^*\mathcal A_3,\qquad q=\pm1.}
$$

Here $\mathcal A_3$ is the super-three-form and $Z^*$ denotes the [pullback of a differential form](../../../../../pullback-of-a-differential-form.md). Its bosonic restriction is the ordinary supergravity potential, but its fermionic components are retained in this action. The magnitude of its [Wess-Zumino brane coupling](../../../../../wess-zumino-brane-coupling.md) equals the membrane tension; the sign $q$ fixes the orientation and the matching sign of $\Gamma_\kappa$. In flat superspace one may take $\Pi^a=dX^a-i\overline\Theta\Gamma^a d\Theta$, with the super-three-form chosen to obey the standard supergravity superspace constraints. Thus this is a fermionic, [kappa symmetry](../../../../../kappa-symmetry.md)-invariant action, rather than merely its bosonic truncation.

To construct an ordinary [calibration](../../../../../calibration-differential-geometry.md), first take a flux-free static background $ds^2=-dt^2+g_{mn}dx^m dx^n$ with a unit covariantly constant spinor $\epsilon$. In a compatible orientation and mostly-plus [Clifford algebra](../../../../../clifford-algebra.md), the membrane [spinor calibration form](../../../../../spinor-calibration-form.md) is

$$
\boxed{\varphi=\frac12\epsilon^\dagger\Gamma_0\Gamma_{ab}\epsilon\;e^a\wedge e^b.}
$$

For an oriented orthonormal spatial pair $u,v$, $\varphi(u,v)=\epsilon^\dagger\Gamma_0\gamma(u)\gamma(v)\epsilon$. The matrix on the right is the static membrane $\Gamma_\kappa$, a Hermitian involution, so this value is at most one, with equality precisely when $\Gamma_\kappa\epsilon=\epsilon$. Parallel transport of the spinor and [gamma matrices](../../../../../gamma-matrices.md) gives $\nabla\varphi=0$, hence $d\varphi=0$.

A [calibration](../../../../../calibration-differential-geometry.md) is a closed [differential form](../../../../../differential-form-split.md) whose value on each oriented unit tangent plane is at most one; its [comass](../../../../../comass.md) is at most one. A [calibrated submanifold](../../../../../calibrated-submanifold.md) $\Sigma$ saturates the bound, $\varphi|_\Sigma=\operatorname{vol}_\Sigma$. For any homologous competitor $\Sigma'$ with the same boundary, [Stokes theorem](../../../../../stokes-theorem.md) gives

$$
\operatorname{Vol}(\Sigma)=\int_\Sigma\varphi
=\int_{\Sigma'}\varphi\leq\operatorname{Vol}(\Sigma').
$$

This proves that [calibration implies volume minimization](../../../../../calibration-implies-volume-minimization.md), and in particular that the membrane's spatial surface is a [minimal surface](../../../../../minimal-surface.md). The closure condition is indispensable. A general flux-coupled [Killing spinor](../../../../../killing-spinor.md) need not produce a closed ordinary [calibration](../../../../../calibration-differential-geometry.md); the corresponding [generalized calibration](../../../../../generalized-calibration.md) bounds the full brane energy including its potential coupling. The flux-free construction above is the ordinary volume-minimizing case.

For the flux-coupled membrane, the standard spinor bilinears give a [Killing vector](../../../../../killing-vector-field.md) $K$ and a two-form $\Omega$ satisfying $d\Omega=\iota_KF$, in matching supergravity conventions. In a stationary gauge $\mathcal L_KA=0$, [Cartan's magic formula](../../../../../cartan-s-magic-formula.md) gives

$$
d(\Omega+\iota_KA)=\iota_KF+\mathcal L_KA-\iota_KdA=0.
$$

This closed charge form provides the membrane [generalized calibration](../../../../../generalized-calibration.md); its potential term is what changes the volume bound into an energy bound.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
