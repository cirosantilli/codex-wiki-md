<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use left-chiral [superfields](../../../../../superfield.md) throughout, abbreviating the conjugate singlets by $U_i=\bar u_i^c$, $D_i=\bar d_i^c$, $E_i=\bar e_i^c$ and $N_i=\bar\nu_i^c$. The printed [hypercharge](../../../../../hypercharge.md) convention is the negative of the usual one, so $Q_{\mathrm{em}}=T_3-Y$; consequently $H_1$ is the down-type and $H_2$ the up-type Higgs doublet. Write $A\cdot B=\epsilon_{\alpha\beta}A^\alpha B^\beta$ for the weak-doublet contraction. Assign [baryon number](../../../../../baryon-number.md) $B(Q)=1/3$, $B(U)=B(D)=-1/3$, and [lepton number](../../../../../lepton-number.md) $L(L)=1$, $L(E)=L(N)=-1$; both Higgs fields have $B=L=0$.

The [baryon number](../../../../../baryon-number.md) and [lepton number](../../../../../lepton-number.md) conserving homogeneous cubic [superpotential](../../../../../superpotential.md) is

$$
\boxed{W_{3,\mathrm{cons}}=(y_u)_{ij}(Q_i\cdot H_2)U_j+(y_d)_{ij}(Q_i\cdot H_1)D_j+(y_e)_{ij}(L_i\cdot H_1)E_j+(y_\nu)_{ij}(L_i\cdot H_2)N_j.}
$$

Each term has zero [hypercharge](../../../../../hypercharge.md), is a color and weak singlet, and has $B=L=0$. Higgs expectation values give the usual [quark](../../../../../quark.md) and charged-lepton [Yukawa interaction](../../../../../yukawa-interaction.md) masses and, here, Dirac [neutrino](../../../../../neutrino.md) masses. The complete remaining cubic part is

$$
\begin{aligned}
W_{3,\mathrm{viol}}={}&\frac12\lambda_{ijk}(L_i\cdot L_j)E_k+\lambda'_{ijk}(L_i\cdot Q_j)D_k\\
&+\frac12\lambda''_{ijk}\epsilon^{abc}U_{i,a}D_{j,b}D_{k,c}
+\kappa_iN_i(H_1\cdot H_2)+\frac16\rho_{ijk}N_iN_jN_k.
\end{aligned}
$$

The first two terms have $\Delta L=+1$, the third has $\Delta B=-1$, the fourth has $\Delta L=-1$, and the last has $\Delta L=-3$. Their Hermitian conjugates reverse these signs. Commutativity of [chiral superfields](../../../../../chiral-superfield.md) and the antisymmetric weak/color contractions give $\lambda_{ijk}=-\lambda_{jik}$ and $\lambda''_{ijk}=-\lambda''_{ikj}$; $\rho$ can be taken completely symmetric. All other coupling [tensors](../../../../../tensor.md) are unrestricted complex [tensors](../../../../../tensor.md).

To check completeness, a cubic [color singlet](../../../../../colour-singlet.md) containing a [quark](../../../../../quark.md) doublet and an [antiquark](../../../../../antiquark.md) singlet must contain a colorless weak doublet; the allowed hypercharges give $QH_2U$, $QH_1D$ and $QLD$. Three color-antitriplet singlets can form a singlet with $\epsilon^{abc}$, but [hypercharge](../../../../../hypercharge.md) permits only $UDD$. Three [quark](../../../../../quark.md) doublets cannot be a weak singlet. With no colored fields, an even number of weak doublets is necessary. Two doublets and a singlet give precisely $LH_1E$, $LLE$, $LH_2N$ and $H_1H_2N$; contractions of two identical Higgs [superfields](../../../../../superfield.md) vanish. With no doublets the only neutral triple is $NNN$. Thus **$W_3=W_{3,\mathrm{cons}}+W_{3,\mathrm{viol}}$ is the most general homogeneous cubic [superpotential](../../../../../superpotential.md)** for the printed fields, including their singlet [neutrinos](../../../../../neutrino.md).

If “cubic” is intended to mean a polynomial of degree at most three, also add

$$
W_{\leq2}=\mu H_1\cdot H_2+\epsilon_iL_i\cdot H_2+\frac12M_{ij}N_iN_j+t_iN_i+W_0,\qquad M_{ij}=M_{ji}.
$$

The $\mu$ term conserves both charges; the other nonconstant terms have respectively $\Delta L=1,-2,-1$. This distinction will matter for the printed claim about [R-parity](../../../../../r-parity.md).

For [squark-mediated proton decay](../../../../../squark-mediated-proton-decay.md), choose $\lambda'_{11k}$ and $\lambda''_{11k}$ with $k=2$ or $3$. The same down-type singlet [squark](../../../../../squark.md) can appear in both vertices; $k=1$ would give $\lambda''_{111}=0$ by antisymmetry. The first term includes an electron/up-quark/[squark](../../../../../squark.md) vertex, and the second an up-quark/down-quark/[squark](../../../../../squark.md) vertex. Exchanging a [squark](../../../../../squark.md) of mass $M$ and expanding its propagator at momenta much smaller than $M$ produces the dimension-six [effective operator](../../../../../effective-operator.md)

$$
\mathcal L_{\mathrm{eff}}\supset C\,\epsilon_{abc}(u_L^a e_L)(u_R^b d_R^c)+\mathrm{h.c.},\qquad C\sim\frac{\lambda'_{11k}\lambda''_{11k}{}^*}{M^2}.
$$

The left- and right-handed pairs are separately contracted spinor bilinears. This operator converts an up/down [quark](../../../../../quark.md) pair into a positron and an [antiquark](../../../../../antiquark.md); the spectator up [quark](../../../../../quark.md) can combine with the [antiquark](../../../../../antiquark.md) into the neutral [pion](../../../../../pion.md). Equivalently its hadronic [matrix](../../../../../matrix.md) element between a [proton](../../../../../proton.md) and a [pion](../../../../../pion.md) is permitted, so it induces $p\to e^+\pi^0$. Having both the [baryon number](../../../../../baryon-number.md) and [lepton number](../../../../../lepton-number.md) violating vertices is what enables this channel.

Since $C$ has mass dimension $-2$, [dimensional analysis](../../../../../dimensional-analysis.md) gives

$$
\boxed{\Gamma(p\to e^+\pi^0)\sim c_h\frac{|\lambda'_{11k}\lambda''_{11k}|^2}{M^4}m_p^5.}
$$

The dimensionless $c_h$ includes the hadronic [matrix](../../../../../matrix.md) element and two-body phase space; the [pion](../../../../../pion.md) mass changes this factor rather than the leading dimensions. Dimensional grounds alone do not give a precise hadronic coefficient. Using the lifetime supplied in the paper, rather than substituting a different bound, gives $\Gamma<1/(2.4\times10^{64})\,\mathrm{GeV}=4.17\times10^{-65}\,\mathrm{GeV}$ and hence

$$
\boxed{|\lambda'_{11k}\lambda''_{11k}|<\frac{M^2}{\sqrt{c_h(2.4\times10^{64}\,\mathrm{GeV}^{-1})m_p^5}}\simeq6.5\times10^{-27}c_h^{-1/2}\left(\frac{M}{1\,\mathrm{TeV}}\right)^2\left(\frac{1\,\mathrm{GeV}}{m_p}\right)^{5/2}.}
$$

For an illustrative $100\,\mathrm{GeV}$ [squark](../../../../../squark.md) this is about $6.5\times10^{-29}c_h^{-1/2}$ when $m_p$ is rounded to $1\,\mathrm{GeV}$. The bound constrains the relevant flavour product and depends on the exchanged mass; separate smallness of each coupling does not follow without an additional assumption.

Define [matter parity](../../../../../matter-parity.md) and [R-parity](../../../../../r-parity.md) by

$$
\boxed{P_M=(-1)^{3(B-L)},\qquad R_p=(-1)^{3(B-L)+2s}=P_M(-1)^{2s}.}
$$

Every matter [superfield](../../../../../superfield.md) $Q,U,D,L,E,N$ has $P_M=-1$, whereas $H_1,H_2$ and the [vector superfields](../../../../../vector-superfield.md) have $P_M=+1$. For ordinary [quarks](../../../../../quark.md) and [antiquarks](../../../../../antiquark.md), $3(B-L)=\pm1$ is odd and $2s=1$, so $R_p=+1$. For charged [leptons](../../../../../lepton.md), [neutrinos](../../../../../neutrino.md) and their antiparticles, $3(B-L)=\mp3$ is odd and $2s=1$, again giving $R_p=+1$; the singlet [neutrino](../../../../../neutrino.md) fermion obeys the same rule. [Gluons](../../../../../gluon.md), the [photon](../../../../../photon.md), $W$ and $Z$ have $B=L=0$ and spin one, hence $R_p=+1$; [Higgs bosons](../../../../../higgs-boson.md) have $B=L=s=0$ and also $R_p=+1$. Thus **every [Standard Model](../../../../../standard-model-split.md) particle is R-even**, including the corresponding antiparticles. Changing spin by one half within a [supermultiplet](../../../../../supermultiplet.md) reverses $R_p$, so [squarks](../../../../../squark.md), [sleptons](../../../../../slepton.md), [gauginos](../../../../../gaugino.md) and [Higgsinos](../../../../../higgsino.md) are R-odd.

Each conserving cubic term contains two R-odd matter [superfields](../../../../../superfield.md) and one even Higgs [superfield](../../../../../superfield.md), so it is even under [matter parity](../../../../../matter-parity.md). Each term in $W_{3,\mathrm{viol}}$ has an odd number of matter [superfields](../../../../../superfield.md): three for $LLE,LQD,UDD,NNN$, and one for $NH_1H_2$. All are therefore forbidden. At the component level the two fermion spin factors in a [Yukawa interaction](../../../../../yukawa-interaction.md) multiply to $+1$, so the same selection rule follows directly from [R-parity](../../../../../r-parity.md). This verifies **all cubic baryon/lepton-number violating terms are forbidden while the Yukawa fermion mass terms survive**.

The blanket assertion needs a qualification beyond homogeneous cubic terms. The Higgs $\mu$ term is even; $L H_2$ and $N$ are odd and forbidden. But $N_iN_j$ is even and permits a Majorana [neutrino](../../../../../neutrino.md) mass despite violating [lepton number](../../../../../lepton-number.md) by two. Likewise the higher-dimensional operators $QQQL$ and $(LH_2)^2$ are even. Consequently [R-parity](../../../../../r-parity.md) alone does not enforce all-order conservation of [baryon number](../../../../../baryon-number.md) and [lepton number](../../../../../lepton-number.md), or absolute [proton](../../../../../proton.md) stability; the stated precise exclusion holds for the violating cubic interactions above.

Two physical implications follow from multiplicative conservation of [R-parity](../../../../../r-parity.md). **[Superpartners](../../../../../sparticle.md) are produced in even numbers from an initial state consisting only of [Standard Model](../../../../../standard-model-split.md) particles**, leading to pair production at the lowest threshold and parity-conserving cascades. **The [lightest supersymmetric particle](../../../../../lightest-supersymmetric-particle.md) is stable**, since one R-odd particle cannot decay exclusively into R-even particles and no lighter R-odd state is available. A neutral weakly interacting [lightest supersymmetric particle](../../../../../lightest-supersymmetric-particle.md) can therefore be a dark-matter candidate and produce missing-energy signatures; neutrality and a suitable abundance require further model assumptions.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
