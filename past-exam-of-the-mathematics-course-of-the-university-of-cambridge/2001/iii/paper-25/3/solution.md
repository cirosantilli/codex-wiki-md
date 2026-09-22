<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use logarithms to base two and set $0\log_2 0=0$. For a [density matrix](../../../../../density-matrix.md) with eigenvalues $(\lambda_j)$, the [Von Neumann entropy](../../../../../von-neumann-entropy-split.md) is

$$
\boxed{S(\rho)=-\operatorname{Tr}(\rho\log_2\rho)=-\sum_j\lambda_j\log_2\lambda_j.}
$$

Thus it is the [Shannon entropy](../../../../../information-entropy.md) of the spectrum. In dimension $d$, each term is nonnegative, and entropy vanishes exactly when one eigenvalue is one, namely for a [pure state](../../../../../pure-state.md). The [Jensen inequality](../../../../../jensen-s-inequality.md) applied to the strictly concave function $-x\log_2x$ gives $S(\rho)\le\log_2d$, with equality precisely at the maximally mixed state $I/d$. Unitary conjugation preserves eigenvalues, so $S(U\rho U^\dagger)=S(\rho)$. Product eigenvalues give

$$
S(\rho\otimes\sigma)=-\sum_{i,j}\lambda_i\mu_j\log_2(\lambda_i\mu_j)=S(\rho)+S(\sigma).
$$

The finite-dimensional entropy is continuous because the eigenvalues depend continuously on the matrix and $-x\log x$ is continuous also at zero.

Define the [partial trace](../../../../../partial-trace.md) over $\mathcal K_2$ by choosing an orthonormal basis $(e_b)$ and setting

$$
\rho_1=\sum_b(I\otimes\langle e_b|)\rho(I\otimes|e_b\rangle).
$$

Equivalently it is uniquely characterized by $\operatorname{Tr}(\rho_1 A)=\operatorname{Tr}(\rho(A\otimes I))$ for every operator $A$ on $\mathcal K_1$. This identity proves basis independence. Define $\rho_2$ similarly, with $\operatorname{Tr}(\rho_2 B)=\operatorname{Tr}(\rho(I\otimes B))$. Hermiticity is preserved by the displayed sum. For each $u\in\mathcal K_1$,

$$
\langle u,\rho_1u\rangle=\sum_b\langle u\otimes e_b,\rho(u\otimes e_b)\rangle\ge0.
$$

Taking the trace in a product orthonormal basis gives $\operatorname{Tr}\rho_1=\operatorname{Tr}\rho=1$, and the same proof works for $\rho_2$. Thus **both reductions are density matrices**. This is the [partial trace positivity from product vectors](../../../../../partial-trace-positivity-from-product-vectors.md) argument.

For a bipartite pure state $\rho=|\psi\rangle\langle\psi|$, expand $\psi$ in a product orthonormal basis with coefficient matrix $C$. A [singular value decomposition](../../../../../singular-value-decomposition.md) gives the [Schmidt decomposition](../../../../../schmidt-decomposition.md)

$$
|\psi\rangle=\sum_{j=1}^r s_j|a_j\rangle\otimes|b_j\rangle,\qquad s_j>0,\quad\sum_js_j^2=1,
$$

with orthonormal families on both sides. Taking the two partial traces makes all cross terms vanish:

$$
\rho_1=\sum_js_j^2|a_j\rangle\langle a_j|,\qquad
\rho_2=\sum_js_j^2|b_j\rangle\langle b_j|.
$$

The spectra may have different numbers of zeros but have identical nonzero eigenvalues. Consequently **the reduced entropies coincide**:

$$
\boxed{S(\rho_1)=S(\rho_2)=-\sum_js_j^2\log_2s_j^2.}
$$

This common value is the [entanglement entropy](../../../../../entanglement-entropy.md). In infinite-dimensional trace-class systems the same partial-trace and Schmidt arguments apply, and the equality remains valid with the value $+\infty$ allowed; the bound $\log_2d$ is specifically finite-dimensional.

For completeness, the basic mixing and correlation properties also admit short proofs. Define [quantum relative entropy](../../../../../quantum-relative-entropy.md) by $D(\tau\|\sigma)=\operatorname{Tr}\tau(\log_2\tau-\log_2\sigma)$ when supports are included, and by $+\infty$ otherwise. Here is its nonnegativity proof without merely citing an operator inequality. Diagonalize $\tau,\sigma$ with eigenvalues $r_i,s_j$, and let $q_{ij}$ be the squared overlaps of their eigenbases. Both row and column sums of $q$ are one. The scalar inequality $r\ln(r/s)\ge r-s$, with zero cases taken by limits, gives

$$
(\ln2)D(\tau\|\sigma)=\sum_{i,j}q_{ij}r_i\ln(r_i/s_j)
\ge\sum_{i,j}q_{ij}(r_i-s_j)=0.
$$

Equality forces $r_i=s_j$ on every nonzero overlap, hence $\tau=\sigma$. For $\overline\rho=\sum_ip_i\rho_i$, expanding the trace definition yields

$$
S(\overline\rho)-\sum_ip_iS(\rho_i)=\sum_ip_iD(\rho_i\|\overline\rho)\ge0,
$$

which proves [Concavity of Von Neumann entropy](../../../../../concavity-of-von-neumann-entropy.md).

The complementary [entropy bounds for a quantum mixture](../../../../../entropy-bounds-for-a-quantum-mixture.md) are

$$
\sum_ip_iS(\rho_i)\le S(\overline\rho)\le H(p)+\sum_ip_iS(\rho_i).
$$

To prove the upper bound, write the spectral pure-state decompositions of the $\rho_i$ as one ensemble with weights $w_{ij}=p_i\lambda_{ij}$. Form the column matrix with columns $\sqrt{w_{ij}}\,|\psi_{ij}\rangle$. Its two Gram operators have the same nonzero spectrum: one is $\overline\rho$, and the other, $G$, has diagonal $w$. Relative entropy against $\operatorname{diag}w$ gives $0\le D(G\|\operatorname{diag}w)=H(w)-S(G)$. Since $H(w)=H(p)+\sum_ip_iS(\rho_i)$ and $S(G)=S(\overline\rho)$, the bound follows. Zero-weight columns are omitted.

Finally the support of $\rho$ is contained in $\operatorname{supp}\rho_1\otimes\operatorname{supp}\rho_2$. Indeed, a vector in a marginal kernel gives a sum of nonnegative product-vector expectations equal to zero; positivity forces the corresponding product vectors into the kernel of $\rho$. The operator identity $\log(\rho_1\otimes\rho_2)=\log\rho_1\otimes I+I\otimes\log\rho_2$ on this support and the partial-trace identities give

$$
0\le D(\rho\|\rho_1\otimes\rho_2)=S(\rho_1)+S(\rho_2)-S(\rho).
$$

This proves [Subadditivity of Von Neumann entropy](../../../../../subadditivity-of-von-neumann-entropy.md), with equality exactly for a product state. Purify $\rho_{12}$ by adjoining a third system, using its spectral decomposition. Equality of pure-state marginal entropies gives $S(\rho_{13})=S(\rho_2)$ and $S(\rho_3)=S(\rho_{12})$. Subadditivity on systems $1,3$ then gives $S(\rho_2)\le S(\rho_1)+S(\rho_{12})$; swapping $1,2$ gives the [Araki–Lieb inequality](../../../../../araki-lieb-inequality.md) $\boxed{|S(\rho_1)-S(\rho_2)|\le S(\rho_{12})}$. These finite-dimensional proofs establish the usual basic entropy bounds, rather than attributing all mixed-state behavior to pure-state Schmidt decompositions.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
