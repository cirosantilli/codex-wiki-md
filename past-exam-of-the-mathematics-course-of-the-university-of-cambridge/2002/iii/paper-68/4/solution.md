<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the printed [hypercharge](../../../../../hypercharge.md) convention; reversing every hypercharge relative to another common convention does not change the gauge invariants. Write $U,D,E,N$ for the singlet [chiral superfields](../../../../../chiral-superfield.md) labelled with a superscript $R$ in the paper, and define the weak-doublet contraction $A\cdot B=\epsilon_{ab}A^aB^b$. The most general homogeneous [cubic superpotential with right-handed-neutrino superfields](../../../../../cubic-superpotential-with-right-handed-neutrino-superfields.md) separates as $W_3=W_{B,L}+W_{\rm viol}$, where

$$
\boxed{W_{B,L}=(y_u)_{ij}(Q_i\cdot H_2)U_j+(y_d)_{ij}(Q_i\cdot H_1)D_j
+(y_e)_{ij}(L_i\cdot H_1)E_j+(y_\nu)_{ij}(L_i\cdot H_2)N_j,}
$$

and

$$
\boxed{\begin{aligned}
W_{\rm viol}={}&\frac12\lambda_{ijk}(L_i\cdot L_j)E_k+\lambda'_{ijk}(L_i\cdot Q_j)D_k\\
&+\frac12\lambda''_{ijk}\epsilon^{abc}U_{ia}D_{jb}D_{kc}
+\eta_iN_i(H_1\cdot H_2)+\frac16\kappa_{ijk}N_iN_jN_k.
\end{aligned}}
$$

Repeated generation and color indices are summed. Because the [chiral superfields](../../../../../chiral-superfield.md) commute while the gauge contractions are antisymmetric,

$$
\lambda_{ijk}=-\lambda_{jik},\qquad \lambda''_{ijk}=-\lambda''_{ikj},\qquad \kappa_{ijk}=\kappa_{(ijk)}.
$$

The factors $1/2$ and $1/6$ remove the corresponding overcounting.

Here is a completeness check, not merely a list of possible terms. A color-singlet cubic can have no colored fields, a fundamental–antifundamental pair, or three fundamentals or three antifundamentals. A colored pair must be $QU$ or $QD$: the remaining weak doublet and [hypercharge](../../../../../hypercharge.md) select respectively $H_2$ or $H_1,L$. Three antifundamentals allow only $UDD$ at zero [hypercharge](../../../../../hypercharge.md); three $Q$ doublets have no weak singlet. With no colored fields, weak invariance requires zero or two doublets. Two positive-hypercharge doublets require $E$, giving $LH_1E$ and $LLE$, while $H_1\cdot H_1=0$. Opposite-hypercharge doublets require $N$, giving $LH_2N$ and $H_1H_2N$. With no doublets, only $NNN$ has zero [hypercharge](../../../../../hypercharge.md). These are exactly the nine structures above.

For [baryon number](../../../../../baryon-number.md) and [lepton number](../../../../../lepton-number.md), assign

$$
B(Q)=\tfrac13,\quad B(U)=B(D)=-\tfrac13,\qquad L(L)=1,\quad L(E)=L(N)=-1,
$$

and zero charges to the Higgs fields. This is the conjugate-singlet convention, so the neutrino [Yukawa coupling](../../../../../yukawa-interaction.md) conserves [lepton number](../../../../../lepton-number.md). The first four terms conserve both charges. The $LLE$ and $LQD$ terms carry $L=1$, the $UDD$ term carries $B=-1$, the $NH_1H_2$ term carries $L=-1$, and $NNN$ carries $L=-3$. The gauge-singlet neutrino interactions must therefore be included in the violating sector.

If “cubic” instead means a polynomial of degree at most three, there are also the lower-degree gauge invariants

$$
W_{\le2}=W_0+t_iN_i+\frac12M_{ij}N_iN_j+\mu H_1\cdot H_2+\mu_iL_i\cdot H_2,\qquad M_{ij}=M_{ji}.
$$

The Higgs mass term conserves both charges; $t_iN_i$, $M_{ij}N_iN_j$ and $\mu_iL_i\cdot H_2$ violate [lepton number](../../../../../lepton-number.md). These additional terms distinguish the full renormalizable [superpotential](../../../../../superpotential.md) from its homogeneous cubic part.

To obtain [squark-mediated proton decay](../../../../../squark-mediated-proton-decay.md), combine a [lepton number](../../../../../lepton-number.md)-violating $LQD$ vertex with a [baryon number](../../../../../baryon-number.md)-violating $UDD$ vertex. A nonzero example is $\lambda'_{112}$ with $\lambda''_{112}$, exchanging the singlet [strange quark](../../../../../strange-quark.md) [squark](../../../../../squark.md) of mass $M_{\widetilde s}$. The antisymmetry forbids $\lambda''_{111}$, so using three first-generation singlets would not be a valid example. The relevant component vertices contain $e_Lu_L\widetilde s^{\,c}$ and $u^cd^c\widetilde s^{\,c}$, with the required color contraction. Connecting one vertex to the complex conjugate of the other through the massive scalar propagator produces schematically

$$
\mathcal L_{\rm eff}\supset\frac{\lambda'_{112}\lambda''^{*}_{112}}{M_{\widetilde s}^2}
\epsilon_{abc}(u_R^a d_R^b)(e_Lu_L^c)+\mathrm{h.c.}
$$

Parentheses denote Lorentz scalar two-spinor contractions, dotted for the right-handed pair and undotted for the left-handed pair. This dimension-six [proton-decay operator](../../../../../proton-decay-operator.md) contains the three quarks $uud$ and an electron field that can create a [Positron](../../../../../positron.md). Its hadronic matrix element $\langle\pi^0|\epsilon_{abc}(u_R^ad_R^b)u_L^c|p\rangle$ gives the channel $p\to e^+\pi^0$. The internal strange flavor need not appear in the final state. The two interactions together violate both continuous charges, as required for this channel.

The coefficient of the dimension-six [effective operator](../../../../../effective-operator.md) has mass dimension $-2$. Thus [dimensional analysis](../../../../../dimensional-analysis.md) gives

$$
\boxed{\Gamma(p\to e^+\pi^0)\sim c_h\,|\lambda'\lambda''|^2\frac{m_p^5}{M_{\widetilde s}^4},\qquad
\tau_p\sim\frac{M_{\widetilde s}^4}{c_h|\lambda'\lambda''|^2m_p^5},}
$$

where $c_h$ is a dimensionless hadronic and phase-space factor. Its detailed value cannot be fixed by dimensional reasoning. Applying the historical lower bound supplied in the paper gives the [proton-lifetime bound on a product of R-parity-violating couplings](../../../../../proton-lifetime-bound-on-a-product-of-r-parity-violating-couplings.md)

$$
\boxed{|\lambda'\lambda''|\lesssim\frac{M_{\widetilde s}^2}{\sqrt{c_h\,(2.4\times10^{64}\,\mathrm{GeV}^{-1})\,m_p^5}}
\simeq\frac{6.5\times10^{-27}}{\sqrt{c_h}}\left(\frac{M_{\widetilde s}}{1\,\mathrm{TeV}}\right)^2\left(\frac{1\,\mathrm{GeV}}{m_p}\right)^{5/2}.}
$$

The numerical coefficient is only the accuracy of the requested dimensional estimate; the squark mass was not fixed by the question.

Finally, [R-parity](../../../../../r-parity.md) is $R_p=(-1)^{3(B-L)+2s}$. At the superfield level use [matter parity](../../../../../matter-parity.md) $P_M=(-1)^{3(B-L)}$: $Q,U,D,L,E,N$ are odd and $H_1,H_2$ are even. Each conserving [Yukawa coupling](../../../../../yukawa-interaction.md) contains two matter [chiral superfields](../../../../../chiral-superfield.md) and one Higgs field, so it is even. Every violating homogeneous cubic above is odd: $LLE,LQD,UDD,NNN$ contain three matter fields, while $NH_1H_2$ contains one. **R-parity forbids all the listed cubic violations and preserves the Yukawa terms that generate fermion masses.** The Higgs bilinear is also even, whereas the lepton bilinear $LH_2$ and the singlet linear term are odd.

The final assertion must not be read as forbidding every possible violation of continuous [baryon number](../../../../../baryon-number.md) or [lepton number](../../../../../lepton-number.md). In particular, [matter parity allows Majorana neutrino masses](../../../../../matter-parity-allows-majorana-neutrino-masses.md): $N_iN_j$ is even but carries $L=-2$, a concrete counterexample once quadratic terms are included. Higher-dimensional operators such as $QQQL$ and $(LH_2)^2$ are likewise even and violate the continuous charges. The verified statement here concerns the homogeneous cubic sector, including the neutrino singlet terms.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
