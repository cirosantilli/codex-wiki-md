<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [BPS state](../../../../../bps-state.md) is a state whose mass saturates a lower bound set by conserved charges in the [Super-Poincaré algebra](../../../../../super-poincare-algebra.md). Saturation leaves some linear combinations of [supercharges](../../../../../supersymmetry-generator.md) unbroken and produces a [shortened massive supermultiplet](../../../../../shortened-massive-supermultiplet.md). Both statements follow from the positivity of the physical Hilbert-space norm, rather than from an assumed classical field configuration.

For four-dimensional [extended supersymmetry](../../../../../extended-supersymmetry.md), choose the normalization

$$
\{Q_\alpha^A,\bar Q_{\dot\beta B}\}=2\delta^A{}_B\sigma^\mu_{\alpha\dot\beta}P_\mu,\qquad \{Q_\alpha^A,Q_\beta^B\}=\epsilon_{\alpha\beta}Z^{AB},\qquad Z^{AB}=-Z^{BA}.
$$

The conjugate algebra is obtained by Hermitian conjugation. The antisymmetry of the [central charge in supersymmetry](../../../../../central-charge-in-supersymmetry.md) matrix follows because the anticommutator is symmetric in the combined labels $(\alpha,A)$ while $\epsilon_{\alpha\beta}$ is antisymmetric. These central charges commute with momentum and [supercharges](../../../../../supersymmetry-generator.md), so their eigenvalues are fixed in an irreducible massive representation. In the rest frame, $P_\mu=(M,0,0,0)$ and $\{Q_\alpha^A,(Q_\beta^B)^\dagger\}=2M\delta^{AB}\delta_{\alpha\beta}$.

For any operator $S$ and physical state $|v\rangle$,

$$
\langle v|\{S,S^\dagger\}|v\rangle=\|S|v\rangle\|^2+\|S^\dagger|v\rangle\|^2\ge0.
$$

Apply this to $S_\alpha^A=Q_\alpha^A-\epsilon_{\alpha\beta}U^{AB}(Q_\beta^B)^\dagger$, where $U$ is unitary. This is the rest-frame version of the positive operator constructed from $Q-\Gamma$. Summing over spinor and internal labels gives

$$
\mathcal H=8\mathcal N M-4\operatorname{Re}\operatorname{tr}(U^\dagger Z)\ge0.
$$

The two diagonal terms each contribute $4\mathcal N M$, because $U^\dagger U=I$; each mixed term contains $\sum_{\alpha\beta}\epsilon_{\alpha\beta}^2=2$. For $\mathcal N=2$, write $Z^{12}=|Z|e^{i\varphi}$ and choose $U=e^{i\varphi}\begin{pmatrix}0&1\\-1&0\end{pmatrix}$. Then $\mathcal H=16M-8|Z|$, so $M\ge|Z|/2$. The factor of one-half reflects the stated convention with $Z$, rather than $2Z$, in the equal-chirality anticommutator.

To obtain the sharp general bound and exhibit the shortening, use [unitary skew-diagonalization of an antisymmetric matrix](../../../../../unitary-skew-diagonalization-of-an-antisymmetric-matrix.md) to put $Z$ into two-by-two blocks $Z_r\begin{pmatrix}0&1\\-1&0\end{pmatrix}$, with a possible zero row and column for odd $\mathcal N$. In one block, relabel its two internal indices $1,2$ and write $Z_r=|Z_r|e^{i\varphi_r}$. Define

$$
a_{r,1}^{\pm}=\frac{Q_1^1\pm e^{i\varphi_r}(Q_2^2)^\dagger}{\sqrt2},\qquad a_{r,2}^{\pm}=\frac{Q_2^1\mp e^{i\varphi_r}(Q_1^2)^\dagger}{\sqrt2}.
$$

Direct substitution, using $\epsilon_{12}=1$, gives

$$
\{a_{r,i}^{\pm},(a_{s,j}^{\pm})^\dagger\}=\delta_{rs}\delta_{ij}(2M\pm|Z_r|),\qquad \{a^+,a^{-\dagger}\}=0,
$$

and all annihilator-annihilator anticommutators vanish. The minus operators must have nonnegative norm in every block, hence the [BPS bound in supersymmetry](../../../../../bps-bound-in-supersymmetry.md) is

$$
\boxed{M\ge\frac12\max_r|Z_r|}.
$$

Equivalently, defining $z_r=Z_r/2$ gives $M\ge\max_r|z_r|$. Applying the positive $Q-\Gamma$ construction to each block gives the same bound; applying only its full trace need not isolate the largest block. For $M>0$ and no central charge saturation, each operator can be normalized by $\sqrt{2M\pm|Z_r|}$ to an ordinary [fermionic annihilation operator](../../../../../fermionic-annihilation-operator.md). The unmatched internal index, if any, contributes two more such operators.

There are consequently $2\mathcal N$ complex creation operators in a generic [massive supermultiplet](../../../../../massive-supermultiplet.md). Starting with a spin-$j$ [Clifford vacuum](../../../../../clifford-vacuum.md), each creation operator can be occupied zero or one times, so the long representation contains $(2j+1)2^{2\mathcal N}$ states. If precisely $k$ central-charge blocks saturate $2M=|Z_r|$, then the two $a_{r,i}^-$ and their adjoints have zero anticommutator. The norm identity forces each of them to annihilate every physical state in that representation. Removing these $2k$ complex oscillators gives

$$
\boxed{\dim\mathcal R_{\mathrm{short}}=(2j+1)2^{2\mathcal N-2k},\qquad 4k\text{ of }4\mathcal N\text{ real supercharges preserved}}.
$$

Thus a massive $\mathcal N=2$ [BPS supermultiplet](../../../../../shortened-massive-supermultiplet.md) is half-BPS. For $j=0$, its four states consist of two spin-zero states and a spin-one-half doublet, instead of the sixteen states of a long representation. A charged representation generally needs its conjugate for [CPT completion of a supermultiplet](../../../../../cpt-completion-of-a-supermultiplet.md), doubling this four-state count; this yields the eight states of a full charged [hypermultiplet](../../../../../hypermultiplet.md). For $\mathcal N=4$, one saturated block gives a quarter-BPS representation and two give a half-BPS representation. This rest-frame argument assumes $M>0$; massless multiplets follow instead from the null-momentum algebra.

The same bound has a geometric realization for solitons. Consider a static [magnetic monopole](../../../../../magnetic-monopole.md) in an $SU(2)$ gauge theory with an adjoint Higgs field $\phi^a$, asymptotic magnitude $v$, vanishing scalar potential and magnetic field $B_i^a$. For magnetic charge $n_m$, the energy can be written

$$
E=\frac12\int d^3x\,(B_i^a\mp D_i\phi^a)^2\pm\int d^3x\,B_i^aD_i\phi^a=\frac12\int d^3x\,(B_i^a\mp D_i\phi^a)^2\pm\frac{4\pi vn_m}{g_{\mathrm{YM}}}.
$$

The second equality uses the covariant magnetic Bianchi identity to turn the cross term into the surface integral $\oint\phi^aB_i^a\,dS_i$. Choosing its sign proves the [Bogomolny bound](../../../../../bogomolny-bound.md) $\boxed{E\ge4\pi v|n_m|/g_{\mathrm{YM}}}$. Equality gives the first-order [Bogomolny equations](../../../../../bogomolny-equations.md) $B_i^a=\pm D_i\phi^a$. In a suitable $\mathcal N=2$ supersymmetric embedding, the surface charge is the appropriate central charge and the soliton obeys precisely the algebraic [BPS bound in supersymmetry](../../../../../bps-bound-in-supersymmetry.md). Its fermionic variation vanishes for the preserved supersymmetry parameters, while the broken [supercharges](../../../../../supersymmetry-generator.md) supply its fermionic zero modes.

Shortening is useful because an isolated short multiplet cannot continuously acquire the additional states of a long representation. While the state exists and stays short, its exact mass is determined by the exact central charge, so masses of strongly interacting solitons can be found without computing a generic interacting-particle self-energy. This does not mean that its numerical mass is independent of coupling or vacuum expectation values: those can enter the central charge itself. Supersymmetric indices and the reduced fermionic state content provide ways to count protected states, subject to possible recombination or continuum effects.

For example, in rank-one [Seiberg–Witten theory](../../../../../seiberg-witten-theory.md) the electric and magnetic charges $(n_e,n_m)$ enter through periods $a,a_D$. In the normalization above, $Z^{12}=2\sqrt2(n_ea+n_ma_D)$, so a [BPS state](../../../../../bps-state.md) has $\boxed{M=\sqrt2|n_ea+n_ma_D|}$. A magnetic monopole can become massless where $a_D=0$, even though the original electric description is strongly coupled. Including this light magnetic [hypermultiplet](../../../../../hypermultiplet.md) supplies a useful local description there; states with both electric and magnetic charge are [dyons](../../../../../dyon.md). Thus the protected spectrum identifies important singularities of the vacuum space and tests electric-magnetic dual descriptions.

The charge bound also controls stability. For any proposed decay with additive complex charges $Z=\sum_i Z_i$, each daughter satisfies $M_i\ge|Z_i|/2$. A BPS parent satisfies

$$
M=\frac{|\sum_iZ_i|}{2}\le\sum_i\frac{|Z_i|}{2}\le\sum_iM_i.
$$

Energy conservation permits decay only if both inequalities are equalities: all daughters must be BPS and their nonzero complex charges must have the same phase. With nonaligned phases the parent lies strictly below the multiparticle threshold. A [wall of marginal stability](../../../../../wall-of-marginal-stability.md) is a locus where such phases align, and a short bound state can disappear across it. Therefore **BPS saturation protects a mass-charge relation and short representation, while stability and existence still depend on the spectrum and parameters**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
