<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use base-two [logarithms](../../../../../../logarithm.md), so [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) is measured in bits, and set $0\log0=0$. Write $D(\rho\Vert\sigma)=\operatorname{Tr}\rho(\log_2\rho-\log_2\sigma)$ for the [quantum relative entropy](../../../../../../quantum-relative-entropy.md), the quantity denoted $S(\rho\Vert\sigma)$ in the paper. It is $+\infty$ unless the [support of a positive operator](../../../../../../support-of-a-positive-operator.md) $\rho$ lies within that of $\sigma$.

We first establish [nonnegativity of quantum relative entropy](../../../../../../nonnegativity-of-quantum-relative-entropy.md), including its equality condition. Let $\rho=\sum_{i:r_i>0}r_i|u_i\rangle\langle u_i|$ and $\sigma=\sum_js_j|v_j\rangle\langle v_j|$, and suppose the support condition holds. Put $q_i=\langle u_i|\sigma|u_i\rangle>0$. Concavity of the scalar logarithm gives

$$
\langle u_i|\log\sigma|u_i\rangle=\sum_j|\langle u_i|v_j\rangle|^2\log s_j\leq\log q_i.
$$

Terms with $s_j=0$ have zero weight here. Working first with natural logarithms, the inequality $-\ln x\geq1-x$ yields

$$
(\ln2)D(\rho\Vert\sigma)\geq\sum_{i:r_i>0}r_i\ln\frac{r_i}{q_i}\geq\sum_{i:r_i>0}(r_i-q_i)\geq0,
$$

since the $q_i$ sum to at most $\operatorname{Tr}\sigma=1$. Equality forces $q_i=r_i$ for every positive-weight eigenvector, no remaining weight of $\sigma$ outside their span, and equality in the logarithm's strict concavity. The latter makes each $u_i$ an eigenvector of $\sigma$ with eigenvalue $q_i$. Thus **$D(\rho\Vert\sigma)=0$ exactly when $\rho=\sigma$**.

For the bipartite [density operator](../../../../../../density-matrix.md),

$$
\operatorname{supp}\rho_{AB}\subseteq\operatorname{supp}\rho_A\otimes\operatorname{supp}\rho_B.
$$

Indeed, a projector onto the kernel of $\rho_A$, tensored with $I_B$, has zero expectation in $\rho_{AB}$. Positivity implies that $\rho_{AB}$ annihilates its range: $\operatorname{Tr}(\rho_{AB}P)=\|\rho_{AB}^{1/2}P\|_{\mathrm{HS}}^2=0$. The same argument applies to $B$. Hence the [quantum relative entropy](../../../../../../quantum-relative-entropy.md) below is finite. On this support,

$$
\log(\rho_A\otimes\rho_B)=(\log\rho_A)\otimes I_B+I_A\otimes\log\rho_B.
$$

Using the [partial trace](../../../../../../partial-trace.md) to evaluate the two local terms gives

$$
D(\rho_{AB}\Vert\rho_A\otimes\rho_B)=S(\rho_A)+S(\rho_B)-S(\rho_{AB})\geq0.
$$

This proves [Subadditivity of Von Neumann entropy](../../../../../../subadditivity-of-von-neumann-entropy.md):

$$
\boxed{S(\rho_{AB})\leq S(\rho_A)+S(\rho_B).}
$$

The proof also identifies equality exactly with the product state $\rho_{AB}=\rho_A\otimes\rho_B$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
