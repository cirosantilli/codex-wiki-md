<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Keep the PDF's [hypercharge](../../../../../hypercharge.md) signs, which are the negatives of the frequently used convention. Write $U,D,E,N$ for the displayed $U^R,D^R,E^R,N^R$ [chiral superfields](../../../../../chiral-superfield.md). Their [gauge group representations](../../../../../gauge-group-representation.md) are conjugate right-handed-matter representations; their [Weyl spinor](../../../../../weyl-spinor.md) components are left-chiral charge conjugates. Thus assign [baryon number](../../../../../baryon-number.md) $B(Q)=\tfrac13$, $B(U)=B(D)=-\tfrac13$, and [lepton number](../../../../../lepton-number.md) $L(L)=1$, $L(E)=L(N)=-1$, with both Higgs fields neutral under $B,L$. The corresponding electromagnetic convention is $Q_{\rm em}=T_3-Y$.

Let $X\cdot Y=\epsilon_{ab}X^aY^b$ contract the two weak doublets, and use the color [Levi-Civita symbol](../../../../../levi-civita-symbol.md) for three color antitriplets. The most general homogeneous [cubic superpotential with right-handed-neutrino superfields](../../../../../cubic-superpotential-with-right-handed-neutrino-superfields.md) separates as $W_3=W_{B,L}+W_{\not B\,\text{or}\,\not L}$, where

$$
\begin{aligned}
W_{B,L}={}&(Y_u)_{ij}(Q_i\cdot H_2)U_j+(Y_d)_{ij}(Q_i\cdot H_1)D_j\\
&+(Y_e)_{ij}(L_i\cdot H_1)E_j+(Y_\nu)_{ij}(L_i\cdot H_2)N_j,
\end{aligned}
$$

and

$$
\begin{aligned}
W_{\not B\,\text{or}\,\not L}={}&\frac12\lambda_{ijk}(L_i\cdot L_j)E_k+\lambda'_{ijk}(L_i\cdot Q_j)D_k\\
&+\frac12\lambda''_{ijk}\epsilon_{rst}U_i^rD_j^sD_k^t+\kappa_iN_i(H_1\cdot H_2)+\frac16\rho_{ijk}N_iN_jN_k.
\end{aligned}
$$

Repeated generation and color indices are summed. The four [Yukawa coupling](../../../../../yukawa-interaction.md) matrices are arbitrary. The weak and color contractions imply $\lambda_{ijk}=-\lambda_{jik}$ and $\lambda''_{ijk}=-\lambda''_{ikj}$, while $\rho_{ijk}$ is completely symmetric. The $\lambda,\lambda'$ terms have $\Delta L=1$; $\lambda''$ has $\Delta B=-1$; $\kappa$ and $\rho$ have respectively $\Delta L=-1,-3$. Their conjugate interactions have the opposite changes. **All four Yukawa terms preserve both numbers; all five remaining types violate at least one.** In particular, the neutral $N$ fields printed in the PDF require both $NH_1H_2$ and $NNN$ terms.

For completeness of this list, a cubic color [gauge-invariant](../../../../../gauge-invariance.md) can contain a $Q$–$U$ or $Q$–$D$ pair and one colorless doublet, or three color antitriplets. Vanishing [hypercharge](../../../../../hypercharge.md) gives $QH_2U$, $QH_1D$, $LQD$ and $UDD$. Three $Q$ doublets have no weak singlet. Among colorless terms, two doublets and a singlet give $LLE$, $LH_1E$, $LH_2N$ and $H_1H_2N$; the apparent $H_1H_1E$ contraction vanishes since the identical bosonic [superfields](../../../../../superfield.md) commute. Three singlets yield only $NNN$. This also explains why no omitted cubic monomial is available. The word cubic excludes the linear $N$ term and the quadratic $H_1H_2$, $L_iH_2$, $N_iN_j$ terms; these are separate possible terms in the full renormalizable [superpotential](../../../../../superpotential.md).

To demonstrate [squark-mediated proton decay](../../../../../squark-mediated-proton-decay.md), take $\lambda'_{11k}$ and $\lambda''_{11k}$ with $k=2$ or $3$. Identical down-flavor indices would make $\lambda''_{111}$ vanish. Both interactions couple to the same scalar $\widetilde D_k$ of mass $M$. Suppressing overall convention-dependent vertex signs, their relevant two-component [fermion](../../../../../fermion.md) bilinears are

$$
\mathcal L_{\rm int}=-\widetilde D_k A-\widetilde D_k^*A^\dagger,\qquad A=\lambda'_{11k}(\nu_e d_L-e_Lu_L)+\lambda''_{11k}\epsilon_{rst}u^{c\,r}d^{c\,s}.
$$

The color index on $A$ is contracted with that on $\widetilde D_k$; Lorentz spinor indices within each bilinear are contracted too. Together with $-M^2|\widetilde D_k|^2$, its algebraic equation at momenta small compared with $M$ gives $\widetilde D_k=-A^\dagger/M^2$. Substitution gives $A^\dagger A/M^2$, whose cross term is the [four-fermion matching for squark-mediated proton decay](../../../../../four-fermion-matching-for-squark-mediated-proton-decay.md)

$$
\mathcal L_{\rm eff}\supset\frac{\lambda'_{11k}\lambda''_{11k}{}^*}{M^2}\epsilon_{rst}(\nu_e d_L^{\,t}-e_Lu_L^{\,t})(u^{c\,r\dagger}d^{c\,s\dagger})+\mathrm{h.c.}
$$

Its electron term contains three quark fields of flavors $uud$ and a lepton, and changes [baryon number](../../../../../baryon-number.md) and [lepton number](../../../../../lepton-number.md) together. The Hermitian-conjugate terms describe both orientations of the process. The hadronic matrix element of the three-quark [proton-decay operator](../../../../../proton-decay-operator.md) between a proton and a neutral pion has the right quantum numbers and is not forbidden by a remaining symmetry. Hence the operator permits $p\to e^+\pi^0$: the lepton field creates the positron and the three-quark matrix element connects the proton to the pion. This supplies the mechanism rather than merely naming the two violating interactions.

Each [fermion](../../../../../fermion.md) field has mass dimension $\tfrac32$, so this [effective operator](../../../../../effective-operator.md) has dimension six and coefficient $C_6=\lambda'\lambda''{}^*/M^2$. By [dimensional analysis](../../../../../dimensional-analysis.md) its contribution to the decay rate has the form

$$
\boxed{\Gamma(p\to e^+\pi^0)\sim c_h\frac{|\lambda'_{11k}\lambda''_{11k}|^2m_p^5}{M^4}.}
$$

Here $c_h$ collects phase space, running and the dimensionless hadronic factor; a dimensional estimate takes it of order unity rather than pretending to calculate a strong-interaction matrix element. Assuming this exchange dominates and there is no tuned cancellation, the supplied lifetime gives the [proton-lifetime bound on a product of R-parity-violating couplings](../../../../../proton-lifetime-bound-on-a-product-of-r-parity-violating-couplings.md)

$$
\boxed{|\lambda'_{11k}\lambda''_{11k}|\lesssim\frac{M^2}{\sqrt{c_h\tau_{\min}m_p^5}}\simeq6.5\times10^{-27}c_h^{-1/2}\left(\frac{M}{1\,\mathrm{TeV}}\right)^2.}
$$

The last estimate uses $m_p\simeq1\,\mathrm{GeV}$ and $\tau_{\min}=2.4\times10^{64}\,\mathrm{GeV}^{-1}$. Keeping $m_p=0.938\,\mathrm{GeV}$ instead changes $6.5$ to about $7.6$. **A numerical limit independent of the squark mass or hadronic factor is not determined by the supplied data.**

Finally, [matter parity](../../../../../matter-parity.md) is $P_M=(-1)^{3(B-L)}$: all matter [chiral superfields](../../../../../chiral-superfield.md), including $N$, are odd, and the Higgs [chiral superfields](../../../../../chiral-superfield.md) are even. [R-parity](../../../../../r-parity.md) of a component field is $R_p=P_M(-1)^{2s}$. In a [superpotential](../../../../../superpotential.md), the spin factor is irrelevant to the allowed monomials: each of $QH_2U,QH_1D,LH_1E,LH_2N$ has two odd matter factors and is even. Each of $LLE,LQD,UDD,NNN$ has three odd matter factors, and $NH_1H_2$ has one, so all are odd and forbidden. Higgs [vacuum expectation values](../../../../../vacuum-expectation-value.md) are even; the allowed [Yukawa interactions](../../../../../yukawa-interaction.md) therefore still generate ordinary [fermion](../../../../../fermion.md) masses.

**R-parity forbids all the baryon/lepton-number-violating cubic terms above, not every possible violating operator.** In particular, $\tfrac12 M_{ij}N_iN_j$ is even under [matter parity](../../../../../matter-parity.md) but changes [lepton number](../../../../../lepton-number.md) by two: [matter parity allows Majorana neutrino masses](../../../../../matter-parity-allows-majorana-neutrino-masses.md). Thus the literal unrestricted claim would be false for these very fields; its valid cubic interpretation gives precisely the requested exclusion while preserving the [Yukawa coupling](../../../../../yukawa-interaction.md) mass terms.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
