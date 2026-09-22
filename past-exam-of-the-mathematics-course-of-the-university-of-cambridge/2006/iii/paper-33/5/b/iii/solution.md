<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Trace out $Q'$ in the final state. With $q(x,y)=p(x)\operatorname{Tr}(E_y\rho_x)$, the remaining state is diagonal in the product classical basis:

$$
\rho_{A'B'}=\sum_{x,y}q(x,y)|x\rangle\langle x|\otimes|y\rangle\langle y|.
$$

The [Von Neumann entropy](../../../../../../../von-neumann-entropy-split.md) of a classical diagonal [density operator](../../../../../../../density-matrix.md) equals the [Shannon entropy](../../../../../../../information-entropy.md) of its diagonal probabilities, by its spectrum. Therefore $I(A':B')=H(X)+H(Y)-H(X,Y)=I(X:Y)$, the [mutual information](../../../../../../../mutual-information.md) between source symbol and measurement outcome.

For the input, put $\bar\rho=\sum_xp(x)\rho_x$. The marginal on $Q$ is $\bar\rho$, the marginal on $A$ has [Von Neumann entropy](../../../../../../../von-neumann-entropy-split.md) $H(X)$, and the [entropy of a classical-quantum state](../../../../../../../entropy-of-a-classical-quantum-state.md) is

$$
S(AQ)=H(X)+\sum_xp(x)S(\rho_x).
$$

To justify the last formula, diagonalize each $\rho_x$ with [eigenvalues](../../../../../../../eigenvalue.md) $\lambda_{xj}$. The joint block-diagonal state has [eigenvalues](../../../../../../../eigenvalue.md) $p(x)\lambda_{xj}$; expanding $-\sum_{x,j}p(x)\lambda_{xj}\log_2[p(x)\lambda_{xj}]$ yields exactly the displayed [Von Neumann entropy](../../../../../../../von-neumann-entropy-split.md). Thus $I(A:Q)=S(\bar\rho)-\sum_xp(x)S(\rho_x)$, the [Holevo quantity](../../../../../../../holevo-quantity.md) of the ensemble. Part (ii) becomes the [Holevo bound](../../../../../../../holevo-s-theorem.md)

$$
\boxed{I(X:Y)\le\chi=S\!\left(\sum_xp(x)\rho_x\right)-\sum_xp(x)S(\rho_x).}
$$

It holds for every POVM, and hence also for the accessible information obtained by maximizing the [mutual information](../../../../../../../mutual-information.md) over all measurements. The only extra [Von Neumann entropy](../../../../../../../von-neumann-entropy-split.md) identities used were the classical-diagonal and classical–quantum block-spectrum formulas, both justified above; the information inequality itself followed from the requested strong-subadditivity argument.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
