<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [Majorana spinor](../../../../../majorana-spinor.md) equals its transform under [charge conjugation](../../../../../charge-conjugation.md), so its spinor components are not independent of their conjugates. In a real two-dimensional [gamma matrix](../../../../../gamma-matrices.md) representation it can be taken real, with anticommuting [Grassmann variables](../../../../../grassmann-variable.md) as components. Each target index labels a separate [worldsheet Majorana fermion](../../../../../worldsheet-majorana-fermion.md); it is not itself a target-space spinor.

Use worldsheet signature $(-,+)$ and the real [gamma matrices](../../../../../gamma-matrices.md)

$$
\gamma^0=\begin{pmatrix}0&-1\\1&0\end{pmatrix},
\qquad
\gamma^1=\begin{pmatrix}0&1\\1&0\end{pmatrix},
\qquad
\{\gamma^\mu,\gamma^\nu\}=2\eta^{\mu\nu}.
$$

Take $\bar\psi=\psi^TC$ with $C=\gamma^0$. Define the [chirality](../../../../../chirality-physics.md) matrix with the chosen worldsheet orientation by

$$
\gamma_*=-\gamma^0\gamma^1=\begin{pmatrix}1&0\\0&-1\end{pmatrix},
\qquad P_\pm=\frac{1\pm\gamma_*}{2}.
$$

It squares to one and anticommutes with each [gamma matrix](../../../../../gamma-matrices.md). [Chirality](../../../../../chirality-physics.md) is its eigenvalue, selected by the [chiral projectors](../../../../../chiral-projector.md). Its overall sign is conventional.

Writing $\psi=(\psi_+,\psi_-)^T$, the fermion [equation of motion](../../../../../equation-of-motion.md) $\gamma^\mu\partial_\mu\psi=0$ becomes

$$
(\partial_\tau+\partial_\sigma)\psi_+=0,\qquad
(\partial_\tau-\partial_\sigma)\psi_-=0.
$$

Hence

$$
\boxed{\psi_+=F(\tau-\sigma)\text{ is right-moving},\qquad
\psi_-=G(\tau+\sigma)\text{ is left-moving}.}
$$

The first profile travels toward increasing $\sigma$, and the second toward decreasing $\sigma$. Thus the choice of [chirality](../../../../../chirality-physics.md) orientation realizes the requested [worldsheet chirality and propagation direction](../../../../../worldsheet-chirality-and-propagation-direction.md) correspondence; reversing the orientation interchanges the labels.

For the rigid [worldsheet supersymmetry](../../../../../worldsheet-supersymmetry.md) variation, let $\epsilon$ be a constant Grassmann-odd [Majorana spinor](../../../../../majorana-spinor.md). With the displayed conventions,

$$
\delta\bar\psi^a=-\bar\epsilon\gamma^\mu\partial_\mu X^a.
$$

The minus sign follows from $(\gamma^\mu)^TC=-C\gamma^\mu$. A second identity from the [Majorana Grassmann bilinear interchange](../../../../../majorana-grassmann-bilinear-interchange.md) is $\bar\chi\gamma^\nu\gamma^\mu\epsilon=\bar\epsilon\gamma^\mu\gamma^\nu\chi$. Keeping these Grassmann signs is essential.

The bosonic kinetic variation is $2i\partial_\mu X_a\,\bar\epsilon\,\partial^\mu\psi^a$. The two fermionic kinetic variations, using the two identities above, give the full result

$$
\begin{aligned}
\delta\mathcal L={}&
2i\partial_\mu X_a\,\bar\epsilon\,\partial^\mu\psi^a
-i\bar\epsilon\gamma^\mu\gamma^\nu\partial_\mu X_a\,\partial_\nu\psi^a
+i\bar\epsilon\psi_a\,\partial_\mu\partial^\mu X^a\\
={}&\partial_\nu\!\left(i\bar\epsilon\gamma^\nu\gamma^\mu
\psi_a\,\partial_\mu X^a\right).
\end{aligned}
$$

For the second equality use $\gamma^\nu\gamma^\mu=2\eta^{\mu\nu}-\gamma^\mu\gamma^\nu$ and symmetry of the second embedding [derivative](../../../../../derivative.md). No field equation has been used. Thus the **variation is an off-shell total [derivative](../../../../../derivative.md)**:

$$
\boxed{\delta I=\int_{\partial\Sigma}d\Sigma_\nu\,
i\bar\epsilon\gamma^\nu\gamma^\mu\psi_a\partial_\mu X^a.}
$$

This is the [rigid worldsheet supersymmetry boundary term](../../../../../rigid-worldsheet-supersymmetry-boundary-term.md). It vanishes when the boundary flux vanishes, for example on a closed worldsheet with compatible fields and variations. On a spatial circle, a constant supersymmetry parameter must also respect the chosen [spin structure](../../../../../spin-structure.md). Periodic fermions allow this rigid transformation; antiperiodic fermions and a constant parameter would give an antiperiodic $\delta X$ and fail to preserve a periodic bosonic embedding. The local action identity remains valid, but global symmetry requires compatible boundary data. This is the [spin-structure obstruction to constant worldsheet supersymmetry](../../../../../spin-structure-obstruction-to-constant-worldsheet-supersymmetry.md).

For the spectrum, assume the usual critical [RNS string](../../../../../spinning-string.md), physical-state constraints, a nonzero null target momentum, and the supersymmetric [GSO projection](../../../../../gso-projection.md). Analyze just one chiral sector. Its matter [central charge](../../../../../central-charge.md) is $d+d/2$; the [bc system](../../../../../bc-system.md) and [superconformal ghosts](../../../../../superconformal-ghost.md) contribute $-26+11$. Therefore $3d/2-15=0$ gives the [critical dimension of the RNS superstring](../../../../../critical-dimension-of-the-rns-superstring.md) $d=10$. [Light-cone gauge in string theory](../../../../../light-cone-gauge-in-string-theory.md) leaves eight transverse bosonic and eight transverse fermionic [string oscillator](../../../../../string-oscillator.md) directions.

In the [Neveu–Schwarz sector](../../../../../neveu-schwarz-sector.md), the normal-ordering intercept is $a_{\rm NS}=1/2$. The massless level is $N=1/2$ and has states

$$
b_{-1/2}^{\,i}|0;k\rangle_{\rm NS},\qquad i=1,\ldots,8.
$$

The [GSO projection](../../../../../gso-projection.md) retains these eight transverse vector polarizations while removing the tachyonic ground state. They are spacetime [bosons](../../../../../boson.md), although the creating [string oscillator](../../../../../string-oscillator.md) is a worldsheet fermion. In covariant language transversality and the longitudinal null-state quotient leave $10-2=8$ polarizations.

In the [Ramond sector](../../../../../ramond-sector.md), bosonic and fermionic [zero-point energies](../../../../../zero-point-energy.md) cancel, so $a_{\rm R}=0$ and the ground states are massless. The eight transverse fermion zero modes obey

$$
\{d_0^i,d_0^j\}=\delta^{ij},\qquad
\Gamma^i=\sqrt2d_0^i,\qquad
\{\Gamma^i,\Gamma^j\}=2\delta^{ij}.
$$

This [Ramond zero-mode Clifford algebra](../../../../../ramond-zero-mode-clifford-algebra.md) acts on a sixteen-dimensional ground-state space. Its two [chirality](../../../../../chirality-physics.md) subspaces each have dimension eight. The [GSO projection](../../../../../gso-projection.md) keeps one, an $8_s$ or $8_c$ spinor of $\operatorname{SO}(8)$, the rotation subgroup of the massless [little group](../../../../../little-group.md). These are spacetime [fermions](../../../../../fermion.md). Equivalently a ten-dimensional [Majorana-Weyl spinor](../../../../../majorana-weyl-spinor.md) has sixteen real components before the massless [Dirac equation](../../../../../dirac-equation.md) reduces the physical polarization count to eight.

Consequently the [massless chiral RNS spectrum after GSO projection](../../../../../massless-chiral-rns-spectrum-after-gso-projection.md) satisfies

$$
\boxed{N_{\rm bosonic}=8=N_{\rm fermionic}.}
$$

The [GSO projection](../../../../../gso-projection.md) is essential: without it, the transverse [Ramond sector](../../../../../ramond-sector.md) would retain both eight-dimensional spinor chiralities. These are counts for one chiral sector, not the tensor-product counts of the full closed-string spectrum.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
