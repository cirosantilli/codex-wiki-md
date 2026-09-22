<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [affine module sheaf](../../../../../affine-module-sheaf.md) construction makes the remaining statements explicit. For $A=k[V]$ and an $A$-module $M$, define

$$
\widetilde M(D(f))=M_f
$$

on the [basis](../../../../../basis.md) of [principal open subsets](../../../../../principal-open-subscheme.md). Restrictions are the natural [localization](../../../../../localization-of-a-ring.md) maps. Equivalently, a section on an arbitrary [open set](../../../../../open-set.md) is a family $s_P\in M_{\mathfrak m_P}$ which near each point is represented by a single fraction $m/f^r$, with $f$ nonvanishing throughout that neighbourhood. This locally representable family construction gives a [sheaf](../../../../../sheaf-mathematics.md); the usual [localization](../../../../../localization-of-a-ring.md) gluing verifies its [quasi-coherence](../../../../../quasi-coherent-sheaf.md). Its [stalk](../../../../../stalk-of-a-sheaf.md) is $M_{\mathfrak m_P}$ and

$$
\boxed{\Gamma(V,\widetilde M)=M}.
$$

This last identification is precisely the standard module-localization gluing on the affine [basis](../../../../../basis.md), not an assertion that arbitrary [sheaves](../../../../../sheaf-mathematics.md) are determined by their global sections.

Now write $A=k[X]$, $B=k[Y]$ and $\alpha=\phi^\#:A\to B$. Let $\mathcal G=\widetilde M$, $\mathcal H=\widetilde N$ for $A$-modules $M,N$, and let $\mathcal F=\widetilde L$ for a $B$-module $L$. The affine versions of the three constructions are

$$
\boxed{\mathcal G\otimes_{\mathcal O_X}\mathcal H\cong\widetilde{M\otimes_A N},\qquad
\phi_*\mathcal F\cong\widetilde{{}_A L},\qquad
\phi^*\mathcal H\cong\widetilde{B\otimes_A N}}.
$$

Here ${}_A L$ denotes restriction of scalars along $\alpha$, whereas the last associated [sheaf](../../../../../sheaf-mathematics.md) lives on $Y$. To verify the tensor-product assertion, localize at every prime: both [stalks](../../../../../stalk-of-a-sheaf.md) are $M_{\mathfrak m}\otimes_{A_{\mathfrak m}}N_{\mathfrak m}$. For the [direct image](../../../../../direct-image-sheaf.md), $\phi^{-1}D(a)=D(\alpha(a))$, and

$$
\Gamma(D(a),\phi_*\widetilde L)=L_{\alpha(a)}=({}_A L)_a.
$$

These equalities identify the [sheaves](../../../../../sheaf-mathematics.md) on a [basis](../../../../../basis.md) and respect restrictions. For the [pullback of a sheaf of modules](../../../../../pullback-of-a-sheaf-of-modules.md), its [stalk](../../../../../stalk-of-a-sheaf.md) at $Q$ is $B_{\mathfrak m_Q}\otimes_A N$, exactly the [stalk](../../../../../stalk-of-a-sheaf.md) of $\widetilde{B\otimes_A N}$. The local tensor maps are compatible, so these [stalk](../../../../../stalk-of-a-sheaf.md) identifications come from an actual [sheaf](../../../../../sheaf-mathematics.md) isomorphism. Thus all three constructions are [quasi-coherent](../../../../../quasi-coherent-sheaf.md) in the stated affine setting.

Finally construct the natural [projection formula for sheaves](../../../../../projection-formula.md) map by sending a local tensor $m\otimes b$ to $b(1\otimes m)$ in the pulled-back [module](../../../../../module-mathematics.md), followed by [direct image](../../../../../direct-image-sheaf.md). In the affine description, the target $\phi_*\phi^*\widetilde M$ is the [sheaf](../../../../../sheaf-mathematics.md) associated with the $A$-module ${}_A(B\otimes_A M)$, while $\widetilde M\otimes_{\mathcal O_X}\phi_*\mathcal O_Y$ corresponds to $M\otimes_A B$. The maps

$$
m\otimes b\longmapsto b\otimes m,\qquad b\otimes m\longmapsto m\otimes b
$$

are inverse $A$-linear maps. Localizing them commutes with every restriction, proving

$$
\boxed{\phi_*\phi^*\widetilde M\cong
\widetilde M\otimes_{\mathcal O_X}\phi_*\mathcal O_Y}.
$$

No flatness assumption on $A\to B$ or finiteness assumption on $M$ is needed.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
