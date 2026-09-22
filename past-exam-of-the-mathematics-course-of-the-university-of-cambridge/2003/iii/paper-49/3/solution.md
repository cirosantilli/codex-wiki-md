<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\varepsilon=i\sigma_2=\left(\begin{smallmatrix}0&1\\-1&0\end{smallmatrix}\right)$, so $\varepsilon^{-1}=-\varepsilon$. Direct multiplication of the [Pauli matrices](../../../../../pauli-matrices.md) gives $\varepsilon\sigma_i^*\varepsilon=\sigma_i$, equivalently $\varepsilon\sigma_i^*\varepsilon^{-1}=-\sigma_i$. For $U=\exp(i\theta_i\sigma_i/2)\in SU(2)$ this implies

$$
\varepsilon U^*\varepsilon^{-1}=U.
$$

Therefore $\phi^c=\varepsilon\phi^*$ transforms as the same weak [fundamental representation](../../../../../fundamental-representation.md) doublet as $\phi$, while complex conjugation reverses its [hypercharge](../../../../../hypercharge.md) to $-1/2$. This is the [Higgs conjugate doublet](../../../../../higgs-conjugate-doublet.md). The [Yukawa coupling](../../../../../yukawa-interaction.md) product $\bar L\phi^cu_R$ is an $SU(2)$ singlet, and its hypercharges add to

$$
-\frac16-\frac12+\frac23=0.
$$

It is consequently [gauge-invariant](../../../../../gauge-invariance.md) and can supply an up-[quark](../../../../../quark.md) mass.

In [unitary gauge](../../../../../unitary-gauge.md), $\phi^c=((v+H)/\sqrt2,0)^T$. Writing $y_u$ for the full arbitrary coefficient of the [Yukawa coupling](../../../../../yukawa-interaction.md) term, its physical form is

$$
\mathcal L_Y=-y_u(v+H)\bar u_Lu_R+\text{Hermitian conjugate},\qquad\boxed{m_u=|y_u|v.}
$$

A one-generation field rephasing makes the mass positive, and its [Higgs boson](../../../../../higgs-boson.md) coupling is $m_u/v$. The printed Yukawa expression has an additional trailing $m$ after $R^+$ which is never defined. If it denotes a constant, absorb it into $y_u=f^+m$; in the conventional dimensionless Yukawa notation without that factor, $y_u=f^+$. It does not affect the gauge-transformation argument.

For three families, use a [singular value decomposition](../../../../../singular-value-decomposition.md) of the two mass matrices: $U_{uL}^\dagger M_uU_{uR}=D_u$ and $U_{dL}^\dagger M_dU_{dR}=D_d$, with positive diagonal entries. The original left-handed weak current then becomes a current between mass eigenstates with

$$
\boxed{V_{\mathrm{CKM}}=U_{uL}^\dagger U_{dL}.}
$$

A complex $3\times3$ matrix has eighteen real parameters, and $U^\dagger U=I$ imposes nine independent real conditions, leaving nine. A generic [unitary matrix](../../../../../unitary-matrix.md) can be built from three complex plane rotations and three diagonal phases: each plane rotation supplies one angle and one phase. Thus these are three rotation angles and six phases. Rephase each of the six Dirac quark mass eigenfields, applying the same phase to its two chiralities so the diagonal masses stay real. A common phase changes no entry of $V$, leaving five effective rephasings. Removing five of the six phases leaves **three angles and one physical phase**. This [CKM parameter counting](../../../../../ckm-parameter-counting.md) assumes generic nondegenerate masses; degeneracies give additional basis freedom.

Exactly massless [neutrinos](../../../../../neutrino.md) have an arbitrary unitary flavor rotation that changes no mass term. After diagonalizing the charged-[lepton](../../../../../lepton.md) mass matrix, choose the neutrino basis with the same left-handed rotation. The apparent lepton charged-current mixing matrix becomes the identity. Thus [mixing of exactly massless neutrinos is removable](../../../../../mixing-of-exactly-massless-neutrinos-is-removable.md); it is not an analogue of physical CKM mixing.

For the requested [CP symmetry](../../../../../cp-symmetry.md) calculation, write $j_{ij}^\mu=\bar u_i\gamma^\mu(1-\gamma^5)d_j$. The supplied [charge conjugation](../../../../../charge-conjugation.md) transformations, with the fermion-reordering sign, give

$$
\bar u\Gamma d\xrightarrow C\bar d\,C\Gamma^TC^{-1}u.
$$

For $\Gamma=\gamma^\mu(1-\gamma^5)$, use $C(\gamma^5)^TC^{-1}=\gamma^5$ and the given [gamma matrix](../../../../../gamma-matrices.md) relation to obtain

$$
j_{ij}^\mu\xrightarrow C-\bar d_j\gamma^\mu(1+\gamma^5)u_i.
$$

Under [parity](../../../../../parity.md), the current acquires the Lorentz parity matrix and $1+\gamma^5$ becomes $1-\gamma^5$. Under [charge conjugation](../../../../../charge-conjugation.md) the charged vector also changes sign and becomes its conjugate. The two minus signs cancel, and the parity matrices cancel in the contracted operator. Consequently

$$
O_{ij}(x)=j_{ij}^\mu(x)W_\mu(x)\xrightarrow{CP}O_{ij}^\dagger(x_P).
$$

With $k=g/(2\sqrt2)$, the interaction is $-k\sum(V_{ij}O_{ij}+V_{ij}^*O_{ij}^\dagger)$. Therefore

$$
\mathcal L_{cc}(V)\xrightarrow{CP}\mathcal L_{cc}(V^*),\qquad\mathcal L_{cc}^{CP}-\mathcal L_{cc}=2ik\sum_{ij}\operatorname{Im}V_{ij}(O_{ij}-O_{ij}^\dagger),
$$

with the transformed density evaluated at $x_P$. This is the [CP transformation of a charged quark current](../../../../../cp-transformation-of-a-charged-quark-current.md).

Physical noninvariance requires a phase that cannot be removed by quark rephasings. The invariant quartet

$$
J=\operatorname{Im}(V_{ud}V_{cs}V_{us}^*V_{cd}^*)=c_{12}c_{23}c_{13}^2s_{12}s_{23}s_{13}\sin\delta
$$

is the [Jarlskog invariant](../../../../../jarlskog-invariant.md), where $s_{ij}=\sin\theta_{ij}$ and $c_{ij}=\cos\theta_{ij}$ in the standard three-angle parametrization. If $J\ne0$, no allowed row/column phases can make the matrix real, and the charged-current interaction violates [CP symmetry](../../../../../cp-symmetry.md). For example all three angles $\pi/4$ with $\delta=\pi/2$ give $J=1/(8\sqrt2)\ne0$.

**The printed noninvariance claim is conditional on a nonzero physical phase.** Arbitrary Yukawa matrices do not force it: $V=I$, or any real [CKM matrix](../../../../../cabibbo-kobayashi-maskawa-matrix.md), gives a CP-invariant charged-current interaction. The correct statement is generic [CP violation](../../../../../cp-violation.md) when the irreducible phase is nontrivial, as explained by [quark rephasing and CP conservation](../../../../../quark-rephasing-and-cp-conservation.md).

Finally a [right-handed neutrino](../../../../../right-handed-neutrino.md) has gauge representation $(\mathbf1,\mathbf1)_0$. Its Lorentz-invariant same-chirality bilinear with the field obtained by [charge conjugation](../../../../../charge-conjugation.md) is therefore a [gauge singlet](../../../../../gauge-singlet.md) and permits a [Majorana mass term](../../../../../majorana-mass-term.md), conventionally

$$
-\frac12M\,\overline{\nu_R^c}\nu_R+\text{Hermitian conjugate}.
$$

The factor $1/2$ is the usual convention for a field paired with itself; it may be absorbed into the printed coefficient. A Higgs Yukawa interaction can independently give a [Dirac mass term](../../../../../dirac-mass-term.md). The Majorana term violates [lepton number](../../../../../lepton-number.md) by two units but preserves the gauge symmetries. Corresponding terms for the other charged [Standard Model](../../../../../standard-model-split.md) [fermions](../../../../../fermion.md) carry nonzero [electric charge](../../../../../electric-charge.md), and [quarks](../../../../../quark.md) also carry nontrivial [color charge](../../../../../color-charge.md). Thus this [gauge-invariant right-handed neutrino Majorana mass](../../../../../gauge-invariant-right-handed-neutrino-majorana-mass.md) is allowed while those charged-fermion analogues are forbidden. Merely introducing a [right-handed neutrino](../../../../../right-handed-neutrino.md) permits mass; vanishing mass coefficients would still leave it massless.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
