<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $X$ and $Y$ for the classical [quantum registers](../../../../../../quantum-register.md) $\widetilde X$ and $\widetilde Y$. By the [quantum mutual information](../../../../../../quantum-mutual-information.md) formula $I(U:V)=S(U)+S(V)-S(UV)$, expanding the right-hand side of the [quantum mutual information balance identity](../../../../../../quantum-mutual-information-balance-identity.md) gives

$$
\begin{aligned}
&I(X:B)+I(XB:D)-I(B:D)\\
&=S(X)+S(B)-S(XB)+S(XB)+S(D)-S(XBD)\\
&\qquad-S(B)-S(D)+S(BD)\\
&=S(X)+S(BD)-S(XBD)=I(X:BD).
\end{aligned}
$$

All [Von Neumann entropies](../../../../../../von-neumann-entropy-split.md) here are evaluated in $\omega$.

We use three facts: [quantum mutual information](../../../../../../quantum-mutual-information.md) is nonnegative by [nonnegativity of quantum relative entropy](../../../../../../nonnegativity-of-quantum-relative-entropy.md); a local [quantum channel](../../../../../../quantum-channel.md) cannot increase it by [data processing for quantum mutual information](../../../../../../data-processing-for-quantum-mutual-information.md); and the [quantum mutual information](../../../../../../quantum-mutual-information.md) of a [classical-quantum state](../../../../../../classical-quantum-state.md) is its ensemble's [Holevo quantity](../../../../../../holevo-quantity.md). Write $\chi(\mathcal T)$ for the [Holevo capacity](../../../../../../holevo-capacity.md), the supremum of the output [Holevo quantity](../../../../../../holevo-quantity.md) over finite input ensembles.

The $XB$ marginal is an output ensemble for $\mathcal E$, with inputs $\rho(x)_A=\operatorname{Tr}_C\rho(x)_{AC}$. Consequently $I(X:B)_\omega\leq\chi(\mathcal E)$. Also $\omega_{XBD}$ is obtained from $\sigma_{XYD}$ by a [quantum channel](../../../../../../quantum-channel.md) on $XY$ which retains $X$ and prepares $B$ from $Y$. Hence

$$
I(XB:D)_\omega\leq I(XY:D)_\sigma.
$$

To bound the latter even for [entangled states](../../../../../../entangled-state.md) $\rho(x)_{AC}$, exhibit the [conditional input ensemble after a local measurement](../../../../../../conditional-input-ensemble-after-a-local-measurement.md). Set

$$
q(y|x)=\operatorname{Tr}[(E_y\otimes I_C)\rho(x)_{AC}],\qquad
\rho_C^{x,y}=\frac{\operatorname{Tr}_A[(\sqrt{E_y}\otimes I_C)\rho(x)_{AC}(\sqrt{E_y}\otimes I_C)]}{q(y|x)}
$$

when $q(y|x)>0$; zero-weight outcomes can be omitted. The numerator is a [positive operator](../../../../../../positive-operator.md), its [trace](../../../../../../matrix-trace.md) is $q(y|x)$, and the $q(y|x)$ sum to one. Thus

$$
\sigma_{XYD}=\sum_{x,y}P_X(x)q(y|x)|x,y\rangle\langle x,y|\otimes\mathcal N(\rho_C^{x,y}).
$$

This is a [classical-quantum state](../../../../../../classical-quantum-state.md) with an output ensemble for $\mathcal N$, so $I(XY:D)_\sigma\leq\chi(\mathcal N)$. Combining these bounds with $I(B:D)_\omega\geq0$ yields

$$
\boxed{I(X:BD)_\omega\leq\chi(\mathcal E)+\chi(\mathcal N),\qquad
\chi(\mathcal E\otimes\mathcal N)\leq\chi(\mathcal E)+\chi(\mathcal N).}
$$

The last step takes the supremum over all input ensembles on $AC$. **The left-hand channel direction is $B\leftarrow A$**, as established in part (i); the printed $A\leftarrow B$ in the last inequality is a typographical reversal. Independent product ensembles also give the reverse inequality, so this proves [Holevo-capacity additivity for entanglement-breaking channels](../../../../../../holevo-capacity-additivity-for-entanglement-breaking-channels.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
