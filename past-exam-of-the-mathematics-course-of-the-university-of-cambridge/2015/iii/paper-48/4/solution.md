<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Complexifying the [Clifford algebra](../../../../../clifford-algebra.md) removes the signature dependence of its representation dimension. Pair the $2k$ [gamma matrices](../../../../../gamma-matrices.md) into operators $a_i,a_i^\dagger$ with $\{a_i,a_j^\dagger\}=\delta_{ij}$ and $\{a_i,a_j\}=0$. The $k$ commuting occupation operators have eigenvalues zero or one. Starting from a [Clifford vacuum](../../../../../clifford-vacuum.md), applying every subset of the $k$ [fermionic creation operators](../../../../../fermionic-creation-operator.md) produces $2^k$ independent states. Conversely, these operators construct matrices on a $2^k$-dimensional space, and their products span its full matrix algebra. Thus an irreducible complex [Clifford algebra](../../../../../clifford-algebra.md) module in $D=2k$ has

$$
\boxed{\dim_{\mathbb C}S_{\rm Dirac}=2^k.}
$$

A general Clifford module is a direct sum of these; the statement concerns the minimal spinor.

The [Lorentz group](../../../../../lorentz-group.md) acts through even Clifford products, $\Sigma^{\mu\nu}=\tfrac14[\Gamma^\mu,\Gamma^\nu]$. More precisely this is a representation of its double cover, the [Spin group](../../../../../spin-group.md). The normalized product $\Gamma_*$ of all $2k$ matrices squares to one and anticommutes with each $\Gamma^\mu$, while commuting with every $\Sigma^{\mu\nu}$. Its eigenspaces are the two [Weyl spinor](../../../../../weyl-spinor.md) representations, so **the Dirac spinor is reducible under the connected spin group**:

$$
\boxed{S_{\rm Dirac}=S_+\oplus S_-,\qquad\dim_{\mathbb C}S_\pm=2^{k-1}.}
$$

Each summand is irreducible. The Clifford module itself remains irreducible because an individual $\Gamma^\mu$ interchanges the summands. In $D=2k+1$ one can use the old $\Gamma_*$ as the additional matrix, with an appropriate phase for its signature. No independent [chirality matrix](../../../../../chirality-matrix.md) remains: the product of all $2k+1$ matrices is central and fixed to a scalar on an irreducible module. There are two choices of this central sign for the complex Clifford algebra, but each restricts to the same irreducible $2^k$-dimensional [spinor representation](../../../../../spin-representation.md) of the connected spin group. **An odd-dimensional spinor has no Weyl splitting.** [Majorana spinor](../../../../../majorana-spinor.md) reality conditions depend additionally on dimension and signature; they must be imposed separately from this complex dimension count.

For the massless field counts, use the rotational part $SO(D-2)$ of the [little group](../../../../../little-group.md) and real physical polarizations. A [massless p-form gauge field](../../../../../massless-p-form-gauge-field.md) has only transverse, antisymmetric components after its gauge redundancy and equations of motion are imposed, giving $\binom{D-2}{p}$ polarizations. A [graviton](../../../../../graviton.md) has a symmetric traceless transverse tensor, giving $(D-2)(D-1)/2-1=D(D-3)/2$. A massless fermion obeys a [Dirac equation](../../../../../dirac-equation.md) which halves its off-shell spinor components. In ten dimensions a [Majorana-Weyl spinor](../../../../../majorana-weyl-spinor.md) has sixteen real components off shell and eight physical components; in nine dimensions a [Majorana spinor](../../../../../majorana-spinor.md) has sixteen off shell and eight physical components; in eleven dimensions a [Majorana spinor](../../../../../majorana-spinor.md) has thirty-two off shell and sixteen physical components. A [gravitino](../../../../../gravitino.md) is a transverse vector-spinor with its gamma trace removed, leaving $(D-3)$ times the corresponding physical spinor dimension. Thus the ten-dimensional [Majorana-Weyl](../../../../../majorana-weyl-spinor.md) [gravitino](../../../../../gravitino.md) has $7\times8=56$ polarizations, the nine-dimensional Majorana [gravitino](../../../../../gravitino.md) has $6\times8=48$, and the eleven-dimensional Majorana [gravitino](../../../../../gravitino.md) has $8\times16=128$.

The common Neveu-Schwarz sector of [type IIA supergravity](../../../../../type-iia-supergravity.md) and [type IIB supergravity](../../../../../type-iib-supergravity.md) consists of a [metric tensor](../../../../../metric-tensor.md), the [Kalb–Ramond field](../../../../../kalb-ramond-field.md) $B_2$, and the [dilaton](../../../../../dilaton.md) $\phi$. Their counts are respectively $35$, $\binom82=28$, and $1$. The Ramond-Ramond sectors and fermions distinguish the theories. In [type IIA supergravity](../../../../../type-iia-supergravity.md) the independent bosonic potentials and counts are

$$
\begin{array}{c|ccccc|c}
\text{field}&g_{MN}&B_2&\phi&C_1&C_3&\text{total}\\\hline
\text{polarizations}&35&28&1&\binom81=8&\binom83=56&128
\end{array}
$$

There are two [Majorana-Weyl](../../../../../majorana-weyl-spinor.md) [gravitini](../../../../../gravitino.md) of opposite [chirality](../../../../../chirality-physics.md), giving $56+56=112$, and two [Majorana-Weyl](../../../../../majorana-weyl-spinor.md) [dilatini](../../../../../dilatino.md) of opposite chirality, giving $8+8=16$. Their total is $128$. With gravitini labelled $\psi^+$ and $\psi^-$, the corresponding dilatini have signs $-$ and $+$ respectively. **Type IIA is nonchiral.**

In [type IIB supergravity](../../../../../type-iib-supergravity.md), the independent bosonic potentials and counts are

$$
\begin{array}{c|cccccc|c}
\text{field}&g_{MN}&B_2&\phi&C_0&C_2&C_4&\text{total}\\\hline
\text{polarizations}&35&28&1&1&\binom82=28&\tfrac12\binom84=35&128
\end{array}
$$

The five-form field strength associated with $C_4$ is a [self-dual differential form](../../../../../self-dual-differential-form.md), so only half the seventy transverse four-form components are independent. In Lorentzian ten dimensions the [Hodge star operator](../../../../../hodge-star-operator.md) on five-forms squares to one, making a real self-duality condition possible. The two [Majorana-Weyl](../../../../../majorana-weyl-spinor.md) [gravitini](../../../../../gravitino.md) have the same chirality and contribute $112$ states. Both Majorana-Weyl [dilatini](../../../../../dilatino.md) have the opposite chirality to those gravitini and contribute $16$ states. **Type IIB is chiral, with $128+128$ bosonic and fermionic polarizations.**

For [dimensional reduction](../../../../../dimensional-reduction.md), retain the massless zero modes on a flat circle, with no flux, gauging or fermion twist. A metric splits into a lower-dimensional metric, one vector and one scalar. An ordinary $p$-form splits into a $p$-form and a $(p-1)$-form, according as it has no compact index or one. This preserves counts by [Pascal's identity](../../../../../pascal-s-rule.md), $\binom{D-2}{p}=\binom{D-3}{p}+\binom{D-3}{p-1}$.

Reducing [type IIA supergravity](../../../../../type-iia-supergravity.md) to nine dimensions gives the following decompositions; each number is a count of physical states:

$$
\begin{array}{c|l|r}
\text{ten-dimensional field}&\text{nine-dimensional fields}&\text{counts}\\\hline
g_{MN}&g_{\mu\nu},\ A_\mu^{\rm metric},\ \rho&27+7+1\\
B_2&B_2,\ A_\mu^B&21+7\\
\phi&\phi&1\\
C_1&A_\mu^C,\ C_y&7+1\\
C_3&C_3,\ C_{\mu\nu y}&35+21
\end{array}
$$

Thus the bosonic [maximal nine-dimensional supergravity](../../../../../maximal-nine-dimensional-supergravity.md) multiplet contains one [graviton](../../../../../graviton.md), three massless vectors, two massless two-forms, one massless three-form and three real scalars, with

$$
\boxed{27+3(7)+2(21)+35+3=128.}
$$

Each ten-dimensional [Majorana-Weyl](../../../../../majorana-weyl-spinor.md) [gravitino](../../../../../gravitino.md) becomes one nine-dimensional Majorana [gravitino](../../../../../gravitino.md) and one Majorana spin-one-half field, giving $56=48+8$. Each ten-dimensional [dilatino](../../../../../dilatino.md) gives one more Majorana spin-one-half field. The fermionic multiplet therefore has two [gravitini](../../../../../gravitino.md) and four spin-one-half fields, with $2(48)+4(8)=128$. The fields belong to one maximal gravity [supermultiplet](../../../../../supermultiplet.md), not separate interacting matter multiplets.

Reducing [type IIB supergravity](../../../../../type-iib-supergravity.md) gives $g_{\mu\nu},A_\mu^{\rm metric},\rho$ from the metric; one two-form and one vector each from $B_2$ and $C_2$; and the two scalars $\phi,C_0$. The four-form potential yields a nine-dimensional four-form and three-form, but the ten-dimensional [self-dual differential form](../../../../../self-dual-differential-form.md) condition relates their field strengths. Retaining either one gives $\binom73=\binom74=35$ independent polarizations, not seventy. The same bosonic count, three scalars, three vectors, two two-forms and one three-form, follows. The fermionic reduction likewise gives two [gravitini](../../../../../gravitino.md) and four spin-one-half fields. These are the same [maximal nine-dimensional supergravity](../../../../../maximal-nine-dimensional-supergravity.md) spectrum, as expected from [T-duality](../../../../../t-duality.md). The spectrum is **nonchiral in nine dimensions**, since the odd-dimensional [spinor representation](../../../../../spin-representation.md) has no independent Weyl chirality; the ten-dimensional distinction is lost on restriction to nine-dimensional Lorentz symmetry.

Eleven-dimensional [supergravity](../../../../../supergravity.md) has a metric with $11(8)/2=44$ states, a three-form with $\binom93=84$, and a Majorana [gravitino](../../../../../gravitino.md) with $128$. For direct reduction on a flat two-torus, write the internal indices as $i=1,2$. The metric gives $g_{\mu\nu}$, two vectors $g_{\mu i}$ and three symmetric components $g_{ij}$; the three-form gives $A_{\mu\nu\rho}$, two two-forms $A_{\mu\nu i}$ and one vector $A_{\mu12}$. Hence

$$
44=27+2(7)+3,\qquad84=35+2(21)+7.
$$

The eleven-dimensional Majorana spinor restricts to two nine-dimensional Majorana spinors. The vector-spinor consequently yields two [gravitini](../../../../../gravitino.md) and four spin-one-half fields, giving $128=2(48)+4(8)$. This is again **the same $128+128$ maximal nine-dimensional multiplet**.

For reduction of massless [type IIA supergravity](../../../../../type-iia-supergravity.md) to four dimensions, use a flat six-torus and retain all zero modes, without flux or projections. Internal indices $i=1,\ldots,6$ give

$$
\begin{array}{c|l|r}
\text{field}&\text{four-dimensional fields}&\text{polarizations}\\\hline
g_{MN}&g_{\mu\nu},\ 6g_{\mu i},\ 21g_{ij}&2+6(2)+21=35\\
B_2&B_{\mu\nu},\ 6B_{\mu i},\ 15B_{ij}&1+6(2)+15=28\\
\phi&\phi&1\\
C_1&C_\mu,\ 6C_i&2+6=8\\
C_3&C_{\mu\nu\rho},\ 6C_{\mu\nu i},\ 15C_{\mu ij},\ 20C_{ijk}&0+6(1)+15(2)+20=56
\end{array}
$$

The multiplicities $21,15,20$ come respectively from a symmetric pair of six internal indices, $\binom62$, and $\binom63$. Before dualizing, this gives one [graviton](../../../../../graviton.md), $28$ vectors, $63$ scalars, seven two-forms and one three-form. The seven two-forms provide seven scalar polarizations, whereas the three-form has no local propagating polarization. Thus the final bosonic spectrum is one [graviton](../../../../../graviton.md), $28$ vectors and $70$ scalars, with $2+56+70=128$ states.

A ten-dimensional [Majorana-Weyl spinor](../../../../../majorana-weyl-spinor.md) decomposes into four four-dimensional Majorana spinors. Each ten-dimensional [gravitino](../../../../../gravitino.md) supplies four four-dimensional [gravitini](../../../../../gravitino.md) and twenty-four spin-one-half fields, with $56=4(2)+24(2)$. Each ten-dimensional [dilatino](../../../../../dilatino.md) supplies four spin-one-half fields, with $8=4(2)$. Together they give eight [gravitini](../../../../../gravitino.md) and fifty-six spin-one-half fields, with $8(2)+56(2)=128$. As a separate check, the [helicity spectrum of a massless supermultiplet](../../../../../helicity-spectrum-of-a-massless-supermultiplet.md) with $\mathcal N=8$ has multiplicities $\binom8j$ at helicity $2-j/2$, giving $1,8,28,56,70,56,28,8,1$. **The reduced theory has the field content of [four-dimensional N=8 supergravity](../../../../../four-dimensional-n-8-supergravity.md), with $128+128$ physical states**, exactly as in ten and eleven dimensions. Other compact manifolds or projections can reduce the number of preserved [supercharges](../../../../../supersymmetry-generator.md); the flat-torus assumption is essential to this spectrum.

Here is the local [two-form scalar duality](../../../../../two-form-scalar-duality.md) including its coupling dependence. For this calculation use signature $(-+++)$, $H_{\mu\nu\rho}=3\partial_{[\mu}B_{\nu\rho]}$, and the contravariant volume tensor $\epsilon^{0123}=+1$. A healthy two-form kinetic term and its first-order form are

$$
\mathcal L_B=-\frac1{12g_B^2}H_{\mu\nu\rho}H^{\mu\nu\rho},\qquad
\mathcal L_1=-\frac1{12g_B^2}H_{\mu\nu\rho}H^{\mu\nu\rho}+\frac16\epsilon^{\mu\nu\rho\sigma}H_{\mu\nu\rho}\partial_\sigma a.
$$

Treat $H$ as independent. Varying $a$ imposes its [Bianchi identity for an Abelian p-form](../../../../../bianchi-identity-for-an-abelian-p-form.md), $\partial_\sigma(\epsilon^{\mu\nu\rho\sigma}H_{\mu\nu\rho})=0$, so locally $H=dB$. Varying $H$ instead yields

$$
H^{\mu\nu\rho}=g_B^2\epsilon^{\mu\nu\rho\sigma}\partial_\sigma a.
$$

Use $\epsilon^{\mu\nu\rho\sigma}\epsilon_{\mu\nu\rho\lambda}=-6\delta^\sigma_\lambda$. The original kinetic term becomes $+(g_B^2/2)(\partial a)^2$, and the multiplier term becomes $-g_B^2(\partial a)^2$. Both terms must be substituted; replacing $H$ only in the original kinetic term would produce the wrong sign. Thus

$$
\boxed{\mathcal L_{\rm dual}=-\frac{g_B^2}{2}\partial_\mu a\,\partial^\mu a.}
$$

At fixed normalization of the Bianchi multiplier, the dual kinetic coefficient is the inverse of the original coefficient: if the scalar convention is $-\tfrac1{2g_a^2}(\partial a)^2$, then $g_a=1/g_B$. A canonical scalar is $g_Ba$ for constant $g_B$, but that rescaling hides the formal coupling inversion and changes any assigned scalar periodicity. For a scalar-dependent positive kinetic matrix $\mathcal G_{IJ}$ of several two-forms, the same calculation gives $-\tfrac12(\mathcal G^{-1})^{IJ}\partial a_I\partial a_J$. Additional topological couplings modify the multiplier's derivative terms but do not change this basic inversion of the two-form kinetic matrix. The [Hodge star operator](../../../../../hodge-star-operator.md) exchanges the two-form [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) and [Bianchi identities for an Abelian p-form](../../../../../bianchi-identity-for-an-abelian-p-form.md) with those of the dual scalars; the duality is local and global flux sectors require separate treatment.

A four-dimensional three-form instead has $F_4=dC_3=f\,\operatorname{vol}_4$. Its equation of motion, $d(g_3^{-2}*F_4)=0$, makes $f/g_3^2$ a spacetime constant. For constant coupling the first-order expression in this convention can be written

$$
\mathcal L_1=\frac{f^2}{2g_3^2}-qf,\qquad \partial_\mu q=0.
$$

Here the first-order construction includes a multiplier $q(F_4-dC_3)$: varying $C_3$ imposes $dq=0$, and the displayed density retains the term fixing the flux normalization. Eliminating $f$ gives $f=g_3^2q$ and $\mathcal L_{\rm eff}=-g_3^2q^2/2$. Thus it can encode a constant-flux contribution to the vacuum energy, but no local massless particle or scalar wave. On the zero-flux perturbative vacuum it contributes no state. **The seven two-forms are scalar duals; the three-form is nondynamical**, which completes the four-dimensional field count without discarding a possible global flux parameter.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
