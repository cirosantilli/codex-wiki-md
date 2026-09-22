<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The opening [change-of-rings tensor quotient](../../../../../change-of-rings-tensor-quotient.md) sends $m\otimes_Rn$ to $m\otimes_An$. The target pairing is [bilinear](../../../../../bilinear-map.md) and $R$-balanced because $\theta(r)m\otimes_An=m\otimes_A\theta(r)n$. On the source, let $A$ act through the first factor; commutativity makes that action compatible with the $R$-balancing relations, and the map is $A$-linear. It is [surjective](../../../../../surjective-function.md): the target is the quotient imposing the additional relations $am\otimes_Rn=m\otimes_Ran$ for every $a\in A$. The construction commutes with [module homomorphisms](../../../../../module-homomorphism.md) in both variables.

The [pullback-direct-image adjunction unit](../../../../../pullback-direct-image-adjunction-unit.md) is obtained locally by pulling a section $h\in\mathcal H(V)$ to $\phi^{-1}V$ and sending it to $1\otimes h$ in $\phi^*\mathcal H(\phi^{-1}V)$. These maps respect restrictions and the $\mathcal O_Y$-actions, hence define

$$
\eta_{\mathcal H}:\mathcal H\longrightarrow\phi_*\phi^*\mathcal H.
$$

For $\mathcal H=\mathcal O_Y$, multiplication identifies $\phi^*\mathcal O_Y$ with $\mathcal O_X$, and $\eta_{\mathcal O_Y}$ is precisely the structure morphism $\phi^\#: \mathcal O_Y\to\phi_*\mathcal O_X$.

To construct the [direct-image tensor comparison](../../../../../direct-image-tensor-comparison.md), on $V\subseteq Y$ send $s\otimes t$, with $s\in\mathcal F(\phi^{-1}V)$ and $t\in\mathcal G(\phi^{-1}V)$, to its tensor section of $\mathcal F\otimes_{\mathcal O_X}\mathcal G$. This pairing is $\mathcal O_Y(V)$-balanced through $\phi^\#$ and is compatible with restrictions. The [universal property of the tensor product of modules](../../../../../universal-property-of-the-tensor-product-of-modules.md) and [sheafification](../../../../../sheafification.md) therefore give

$$
\phi_*\mathcal F\otimes_{\mathcal O_Y}\phi_*\mathcal G\longrightarrow\phi_*(\mathcal F\otimes_{\mathcal O_X}\mathcal G).
$$

Apply this with $\mathcal G=\phi^*\mathcal H$ after tensoring the unit $\eta_{\mathcal H}$ with $\phi_*\mathcal F$. The composite is the map in the [projection formula for sheaves](../../../../../projection-formula.md). If $\mathcal H|_V\cong\mathcal O_V^r$, then $\phi^*\mathcal H|_{\phi^{-1}V}\cong\mathcal O_{\phi^{-1}V}^r$, and the composite identifies with

$$
(\phi_*\mathcal F|_V)^{\oplus r}\longrightarrow\phi_*(\mathcal F^{\oplus r})|_V,
$$

the identity on the $r$ components. Thus it is an [isomorphism](../../../../../isomorphism.md) for a [locally free sheaf](../../../../../locally-free-sheaf.md) of finite rank. Neither $\mathcal F$ nor $\mathcal G$ was assumed [quasi-coherent](../../../../../quasi-coherent-sheaf.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
