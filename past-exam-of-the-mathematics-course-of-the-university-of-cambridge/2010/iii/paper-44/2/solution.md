<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the free-boson [operator product expansion](../../../../../operator-product-expansion.md)

$$
X^\mu(z,\bar z)X^\nu(w,\bar w)\sim-\frac{\alpha'}2\eta^{\mu\nu}\log|z-w|^2.
$$

Write $E_p=:e^{ip\cdot X}:$ and $\epsilon=z-w$. The needed [Wick contractions](../../../../../wick-contraction.md) are $\partial X^\mu(z)\partial X^\nu(w)\sim-\alpha'\eta^{\mu\nu}/(2\epsilon^2)$ and $\partial X^\mu(z)E_p(w)\sim-i\alpha'p^\mu E_p(w)/(2\epsilon)$. For $V_\zeta=\zeta_\mu:\partial X^\mu E_p:$, the cross double contraction in the [worldsheet stress tensor](../../../../../worldsheet-stress-energy-tensor.md) has a cubic pole: either of its two derivatives can contract with the derivative in $V_\zeta$, while the other contracts with $E_p$. Including the factor $-1/\alpha'$ gives

$$
T(z)V_\zeta(w)\sim-\frac{i\alpha'}2\frac{p\cdot\zeta}{\epsilon^3}E_p(w)+\frac{1+\alpha'p^2/4}{\epsilon^2}V_\zeta(w)+\frac1\epsilon\partial V_\zeta(w).
$$

A [primary operator](../../../../../primary-field.md) has no cubic pole. Hence **the first vertex is primary precisely when**

$$
\boxed{p\cdot\zeta=0,\qquad h=1+\alpha'p^2/4.}
$$

The antiholomorphic [conformal weight](../../../../../conformal-weight.md) is $\bar h=\alpha'p^2/4$. Primarity alone puts no [mass-shell condition](../../../../../string-mass-shell-condition.md) on $p$.

For $W_\zeta=\zeta_{\mu\nu}:\partial X^\mu\bar\partial X^\nu E_p:$, the holomorphic cubic pole is $-i\alpha'p^\mu\zeta_{\mu\nu}:\bar\partial X^\nu E_p:/(2\epsilon^3)$. The antiholomorphic [operator product expansion](../../../../../operator-product-expansion.md) gives the analogous pole involving $p^\nu\zeta_{\mu\nu}$. Thus the [transversality of derivative-exponential primary vertices](../../../../../transversality-of-derivative-exponential-primary-vertices.md) requires

$$
\boxed{p^\mu\zeta_{\mu\nu}=0,\qquad p^\nu\zeta_{\mu\nu}=0,\qquad (h,\bar h)=(1+\alpha'p^2/4,1+\alpha'p^2/4).}
$$

There is no trace-free requirement for primarity. A physical [integrated string vertex operator](../../../../../integrated-string-vertex-operator.md) must additionally have [conformal weights](../../../../../conformal-weight.md) $(1,1)$; for this vertex that gives $p^2=0$.

Now keep the [fermionic signs](../../../../../fermionic-sign.md) in the real chiral [Majorana fermion](../../../../../majorana-spinor.md) calculation. Contracting the external $\psi(w)$ through $:\psi(z)\partial\psi(z):$ gives

$$
:\psi(z)\partial\psi(z):\,\psi(w)\sim-\frac{\partial\psi(z)}{\epsilon}-\frac{\psi(z)}{\epsilon^2}.
$$

Multiplying by $-1/2$ and Taylor expanding $\psi(z)$ at $w$ produces

$$
T(z)\psi(w)\sim\frac{\psi(w)}{2\epsilon^2}+\frac{\partial\psi(w)}\epsilon.
$$

This proves that $\psi$ is a [primary operator](../../../../../primary-field.md) with **weight $h_\psi=1/2$**. To find the [central charge](../../../../../central-charge.md), in $T(z)T(w)$ the two double-contraction pairings contribute, before the overall factor $1/4$,

$$
-\langle\psi(z)\psi(w)\rangle\langle\partial\psi(z)\partial\psi(w)\rangle=\frac2{\epsilon^4},\qquad \langle\psi(z)\partial\psi(w)\rangle\langle\partial\psi(z)\psi(w)\rangle=-\frac1{\epsilon^4}.
$$

The single [Wick contractions](../../../../../wick-contraction.md) give $2T(w)/\epsilon^2+\partial T(w)/\epsilon$, so

$$
T(z)T(w)\sim\frac1{4\epsilon^4}+\frac{2T(w)}{\epsilon^2}+\frac{\partial T(w)}\epsilon.
$$

Comparing the leading term with $c/(2\epsilon^4)$ proves **$c_\psi=1/2$**, as in the [free chiral Majorana fermion conformal field theory](../../../../../free-chiral-majorana-fermion-conformal-field-theory.md).

With four embedding bosons and the ordinary reparameterization [bc ghost system](../../../../../bc-system.md), cancellation of the [worldsheet Weyl anomaly](../../../../../worldsheet-weyl-anomaly.md) in each chirality requires

$$
4+\frac{N_f}2-26=0,\qquad\boxed{N_f=44.}
$$

Thus there are **44 real left-moving and 44 real right-moving fermions**, equivalently 44 two-dimensional nonchiral [Majorana fermions](../../../../../majorana-spinor.md). These are [internal free fermions in a four-dimensional bosonic string](../../../../../internal-free-fermions-in-a-four-dimensional-bosonic-string.md). Adding internal matter to the bosonic string does not introduce local [worldsheet supersymmetry](../../../../../worldsheet-supersymmetry.md) or its superghosts.

For the requested polynomial [string vertex operators](../../../../../string-vertex-operator.md), work in the unprojected [Neveu–Schwarz sector](../../../../../neveu-schwarz-sector.md). A full model also chooses spin structures and a consistent projection, which the central-charge condition alone does not specify. If the holomorphic and antiholomorphic oscillator contributions to the [conformal weights](../../../../../conformal-weight.md) are $\ell_L,\ell_R$, physicality requires

$$
\ell_L+\frac{\alpha'p^2}4=\ell_R+\frac{\alpha'p^2}4=1,\qquad M^2=\frac4{\alpha'}(\ell_L-1),\qquad \ell_L=\ell_R.
$$

Therefore only equal levels at most one can contribute to the requested nonpositive [bosonic string mass spectrum](../../../../../bosonic-string-mass-spectrum.md).

With zero fermion insertions, level zero gives the [tachyon vertex operator](../../../../../tachyon-vertex-operator.md) $E_p$, a scalar with $M^2=-4/\alpha'$. Level one gives the [massless closed-string vertex operator](../../../../../massless-closed-string-vertex-operator.md) $\zeta_{\mu\nu}:\partial X^\mu\bar\partial X^\nu E_p:$, with the transverse conditions above and the [string-state gauge redundancy](../../../../../string-state-gauge-redundancy.md) that removes longitudinal polarizations. The physical transverse [polarization tensor](../../../../../polarization-tensor.md) decomposes into a symmetric trace-free [graviton](../../../../../graviton.md), an antisymmetric [Kalb–Ramond field](../../../../../kalb-ramond-field.md), and a scalar [dilaton](../../../../../dilaton.md). In four spacetime dimensions these have respectively two, one, and one physical polarizations; the two-form can be dualized to a scalar.

With two fermion insertions there are two possibilities. One fermion in each chirality gives

$$
C_{ij}:\psi^i\bar\psi^j E_p:,qquad (\ell_L,\ell_R)=(1/2,1/2),\qquad \boxed{M^2=-2/\alpha'.}
$$

These are **$44^2=1936$ scalar tachyons** before any projection. There is no spacetime derivative or spacetime polarization to impose a vector transversality condition.

Two different fermions in the same chirality form an antisymmetric [fermion bilinear](../../../../../fermion-bilinear.md), a weight-one current $J^{ij}=: \psi^i\psi^j:$; equal-species undifferentiated bilinears vanish. [Closed-string level matching](../../../../../closed-string-level-matching.md) then requires a weight-one bosonic derivative in the opposite chirality. The resulting [string vertex operators](../../../../../string-vertex-operator.md) are

$$
A^{ij}_\mu:\psi^i\psi^j\bar\partial X^\mu E_p:,qquad \widetilde A^{ij}_\mu:\partial X^\mu\bar\psi^i\bar\psi^j E_p:,qquad i<j.
$$

They have **$M^2=0$ and are gauge vectors**, with $p\cdot A^{ij}=0$ and $A^{ij}_\mu\sim A^{ij}_\mu+p_\mu\lambda^{ij}$, and likewise for $\widetilde A$. Each chirality supplies $\binom{44}{2}=946$ gauge vectors. The [fermion bilinears](../../../../../fermion-bilinear.md) generate the two $\mathfrak{so}(44)$ current algebras associated with the [Special orthogonal Lie algebra](../../../../../special-orthogonal-lie-algebra.md), giving the unprojected [gauge group](../../../../../gauge-group.md) $SO(44)_L\times SO(44)_R$. The tempting vertex $:\psi^i\psi^j E_p:$ alone fails [closed-string level matching](../../../../../closed-string-level-matching.md) because its weights are $(1,0)$ before the common momentum contribution. Additional derivatives raise the levels above the nonpositive-mass range; a product of a left and a right bilinear has four fermion insertions and is outside this requested sector. This completes the [zero- and two-fermion vertices of an internally fermionized bosonic string](../../../../../zero-and-two-fermion-vertices-of-an-internally-fermionized-bosonic-string.md); a specified global projection can remove some of the listed states.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
