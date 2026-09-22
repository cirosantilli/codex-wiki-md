<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $e_A=\varepsilon_{FA}F\eta_A$. This is a [natural transformation](../../../../../../natural-transformation.md) $F\Rightarrow F$. Only the $G$-triangle $G\varepsilon_D\eta_{GD}=1_{GD}$ is assumed. Naturality gives two useful absorption identities:

$$
\begin{aligned}
Ge_A\eta_A
&=G\varepsilon_{FA}GF\eta_A\eta_A
=G\varepsilon_{FA}\eta_{GFA}\eta_A=\eta_A,\\
\varepsilon_D e_{GD}
&=\varepsilon_D\varepsilon_{FGD}F\eta_{GD}
=\varepsilon_DFG\varepsilon_DF\eta_{GD}=\varepsilon_D.
\end{aligned}
$$

For the second equality in the last line use naturality of $\varepsilon$ at $\varepsilon_D$, and then the assumed $G$-triangle. Naturality of $\varepsilon$ at $F\eta_A$ and of $\eta$ at $\eta_A$ now gives

$$
\begin{aligned}
e_A^2
&=\varepsilon_{FA}\varepsilon_{FGFA}FGF\eta_A F\eta_A\\
&=\varepsilon_{FA}\varepsilon_{FGFA}F\eta_{GFA}F\eta_A
=\varepsilon_{FA}e_{GFA}F\eta_A=e_A.
\end{aligned}
$$

Hence **$e$ is an idempotent in the functor category**: this is the [one-triangle adjunction idempotent](../../../../../../one-triangle-adjunction-idempotent.md).

For the [splitting of an idempotent morphism](../../../../../../splitting-of-an-idempotent-morphism.md), suppose this [idempotent morphism](../../../../../../idempotent-morphism.md) splits as [natural transformations](../../../../../../natural-transformation.md) $r:F\Rightarrow H$ and $s:H\Rightarrow F$, with $sr=e$ and $rs=1_H$. Define

$$
\eta'_A=Gr_A\eta_A,\qquad \varepsilon'_D=\varepsilon_Ds_{GD}.
$$

The first absorption identity gives

$$
G\varepsilon'_D\eta'_{GD}
=G\varepsilon_DGe_{GD}\eta_{GD}=1_{GD}.
$$

For the other triangle, naturality of $s$ at $\eta'_A$ and of $\varepsilon$ at $r_A$ gives

$$
\begin{aligned}
\varepsilon'_{HA}H\eta'_A
&=\varepsilon_{HA}s_{GHA}H\eta'_A
=\varepsilon_{HA}F\eta'_A s_A\\
&=\varepsilon_{HA}FGr_A F\eta_A s_A
=r_A\varepsilon_{FA}F\eta_A s_A
=r_Ae_As_A=1_{HA}.
\end{aligned}
$$

Thus the [triangle identities for an adjunction](../../../../../../triangle-identities-for-an-adjunction.md) prove $H\dashv G$.

Conversely, suppose $H\dashv G$, with unit $\psi:1_{\mathcal C}\Rightarrow GH$ and counit $\varphi:HG\Rightarrow1_{\mathcal D}$. The unit has target $GH$, as its type requires. Define

$$
\boxed{s_A=\varphi_{FA}H\eta_A:HA\to FA,\qquad
r_A=\varepsilon_{HA}F\psi_A:FA\to HA.}
$$

These are [natural transformations](../../../../../../natural-transformation.md). Transposition under $H\dashv G$ gives $Gs_A\psi_A=\eta_A$. Independently, naturality of $\eta$ at $\psi_A$ and the assumed $G$-triangle give

$$
Gr_A\eta_A=G\varepsilon_{HA}GF\psi_A\eta_A
=G\varepsilon_{HA}\eta_{GHA}\psi_A=\psi_A.
$$

The transpose of $r_As_A$ is therefore $Gr_AGs_A\psi_A=\psi_A$, the transpose of $1_{HA}$. Injectivity of the hom-set [bijection](../../../../../../bijection.md) implies $r_As_A=1_{HA}$. Naturality of $\varepsilon$ at $s_A$ gives

$$
s_Ar_A=\varepsilon_{FA}FGs_AF\psi_A
=\varepsilon_{FA}F(Gs_A\psi_A)=\varepsilon_{FA}F\eta_A=e_A.
$$

Consequently **$G$ has a left adjoint if and only if $e$ splits**. This is the criterion for [splitting a one-triangle adjunction idempotent](../../../../../../splitting-a-one-triangle-adjunction-idempotent.md). The argument gives both the explicit splitting and the new unit and counit, without assuming the other triangle for $F$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
