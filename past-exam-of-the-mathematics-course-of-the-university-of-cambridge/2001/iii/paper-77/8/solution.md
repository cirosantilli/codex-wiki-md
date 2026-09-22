<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

A [skew Young diagram](../../../../../skew-young-diagram.md) is connected when any two of its cells can be joined by a sequence of cells sharing edges; touching only at a corner does not connect them. A nonempty [border strip](../../../../../rim-hook.md), or [rim hook](../../../../../rim-hook.md), is a connected skew diagram containing no $2\times2$ square. Its height is its number of occupied rows minus one.

For a weak composition $\alpha=(\alpha_1,\ldots,\alpha_\ell)$, a [border-strip tableau](../../../../../border-strip-tableau.md) of shape $\lambda/\mu$ and type $\alpha$ is a chain

$$
\mu=\lambda^{(0)}\subseteq\lambda^{(1)}
\subseteq\cdots\subseteq\lambda^{(\ell)}=\lambda,
$$

whose $i$th difference is a [border strip](../../../../../rim-hook.md) of size $\alpha_i$. Filling that strip with $i$ gives the equivalent weakly increasing row-and-column filling. A zero part corresponds to an empty difference and has height zero. Put $\operatorname{ht}(T)=\sum_i\operatorname{ht}(\lambda^{(i)}/\lambda^{(i-1)})$. For positive $r$, $p_r=\sum_jx_j^r$; write $p_\alpha=\prod_{\alpha_i>0}p_{\alpha_i}$. Thus zero type parts are ignored: one does not multiply by the finite-variable value $p_0=N$.

We first prove the one-strip multiplication formula using [alternants](../../../../../monomial-alternant.md). Choose $N$ sufficiently large and let $\beta_i=\mu_i+N-i$ be the decreasing [beta numbers of a partition](../../../../../beta-number-of-a-partition.md). Expanding the [determinant](../../../../../determinant.md) by [permutations](../../../../../permutation.md) shows

$$
p_r a_\beta
=\sum_{i=1}^N a_{(\beta_1,\ldots,\beta_i+r,\ldots,\beta_N)}.
$$

Indeed, in each [determinant](../../../../../determinant.md) [monomial](../../../../../monomial.md) every variable occurs in exactly one row factor; multiplying that variable by its $r$th power is equivalent to raising that row exponent.

A term vanishes if the new exponent equals another exponent. Otherwise suppose the changed exponent moves from position $i$ to position $j\le i$ when restored to decreasing order. Its [determinant](../../../../../determinant.md) sign is $(-1)^{i-j}$. The resulting partition $\lambda$ has

$$
\lambda_j=\mu_i+r-i+j,\qquad
\lambda_t=\mu_{t-1}+1\quad(j<t\le i),
$$

and all other rows unchanged. The new diagram contains $\mu$, and its size increases by $r$. Between successive added rows, the overlap is exactly the single column $\mu_{t-1}+1$. Thus the added cells form a connected strip without a $2\times2$ square, of height $i-j$. Conversely every added [border strip](../../../../../rim-hook.md) has consecutive occupied rows and exactly this single-column overlap, forcing these formulas and the corresponding exponent shift. The correspondence is therefore bijective. Divide by the unchanged [Vandermonde determinant](../../../../../vandermonde-determinant.md) and use the [bialternant formula](../../../../../bialternant-formula.md) to get the [power-sum border-strip multiplication](../../../../../power-sum-border-strip-multiplication.md) identity

$$
\boxed{p_rs_\mu=
\sum_{\substack{\lambda\supseteq\mu\\
\lambda/\mu\text{ border strip},\ |\lambda|-|\mu|=r}}
(-1)^{\operatorname{ht}(\lambda/\mu)}s_\lambda.}
$$

Apply this formula successively to each positive part of $\alpha$. Each sequence of choices is exactly a [border-strip tableau](../../../../../border-strip-tableau.md), and its product of signs is $(-1)^{\operatorname{ht}(T)}$. Therefore

$$
\boxed{s_\mu p_\alpha
=\sum_\lambda\chi^{\lambda/\mu}(\alpha)s_\lambda,\qquad
\chi^{\lambda/\mu}(\alpha)=\sum_T(-1)^{\operatorname{ht}(T)}.}
$$

Commutativity of the power sums also shows that the resulting coefficient does not depend on the order of the positive parts of the type.

Take $\mu$ empty and restrict to $N\ge\ell(\lambda)$ variables. Multiply by $a_\delta$, with $\delta=(N-1,\ldots,0)$:

$$
p_\alpha a_\delta=\sum_\nu\chi^\nu(\alpha)a_{\nu+\delta}.
$$

In an alternant $a_{\nu+\delta}$, the exponents are distinct and their decreasing arrangement is $\nu+\delta$. Consequently the [monomial](../../../../../monomial.md) $x^{\lambda+\delta}$ occurs only for $\nu=\lambda$, and in that [determinant](../../../../../determinant.md) its coefficient is one. This proves the [Frobenius alternant character formula](../../../../../frobenius-alternant-character-formula.md)

$$
\boxed{\chi^\lambda(\alpha)=[x^{\lambda+\delta}]\,p_\alpha a_\delta.}
$$

To identify these coefficients with symmetric-group characters, recall the [Frobenius characteristic map](../../../../../frobenius-characteristic-map.md)

$$
\operatorname{ch}(\psi)=\sum_{\rho\vdash d}\frac{\psi(\rho)}{z_\rho}p_\rho,
\qquad d=|\alpha|.
$$

The representation-theoretic identification $\operatorname{ch}(\chi^\lambda)=s_\lambda$ can be justified by [Young's rule](../../../../../young-s-rule.md): the [permutation character](../../../../../permutation-character.md) on ordered blocks of sizes $\nu$ is $\sum_\lambda K_{\lambda\nu}\chi^\lambda$. Its characteristic is $h_\nu$, because its fixed block decompositions allocate whole cycles to blocks, and the exponential generating series for those allocations is $\prod_jH(t_j)$. On the symmetric-function side, Hall duality and Schur orthonormality give $h_\nu=\sum_\lambda K_{\lambda\nu}s_\lambda$. Inverting the unitriangular Kostka [matrix](../../../../../matrix.md) establishes the identification. Thus the coefficient of $s_\lambda$ in $p_\rho$ is the irreducible character value on cycle type $\rho$. We have supplied the border-strip computation rather than assuming the character rule.

Grouping border-strip chains by their first removal of a cycle length $r$ now yields the [Murnaghan–Nakayama rule](../../../../../murnaghan-nakayama-rule.md)

$$
\boxed{\chi^\lambda(r,\rho)=
\sum_{\substack{\nu\subseteq\lambda\\\lambda/\nu\text{ border strip of size }r}}
(-1)^{\operatorname{ht}(\lambda/\nu)}\chi^\nu(\rho).}
$$

One may choose the $r$-cycle to be last in a strip-building chain because the power sums commute. The empty-shape value on the empty type is one, providing the recursion's initial condition.

For the staircase $\delta=(m-1,m-2,\ldots,1)$, use $m$ beta numbers including its padded zero row. Its beta set is

$$
\{0,2,4,\ldots,2m-2\}.
$$

Removing a [rim hook](../../../../../rim-hook.md) of length $r$ lowers one beta number by $r$ into an unoccupied nonnegative position, reversing the exponent-shift description above. For a positive even $r$, this move either hits another occupied even position or goes below zero. Therefore there are no removable even-size [border strips](../../../../../rim-hook.md).

Under the [Hall inner product of symmetric functions](../../../../../hall-inner-product-of-symmetric-functions.md), the adjoint of multiplication by $p_r$ is $r\,\partial/\partial p_r$: this follows on the power-sum [basis](../../../../../basis.md) from $z_\nu/z_{\nu\setminus r}=r\,m_r(\nu)$. Taking adjoints of the one-strip multiplication rule expresses this derivative on $s_\delta$ as the signed sum over removable size-$r$ strips. That sum is empty for even $r$, so

$$
\frac{\partial s_\delta}{\partial p_{2r}}=0\quad(r\ge1).
$$

The rational symmetric-function algebra is freely generated by the power sums, and its characteristic is zero. Vanishing of each of these derivatives therefore proves the [staircase Schur functions use only odd power sums](../../../../../staircase-schur-functions-use-only-odd-power-sums.md) statement:

$$
\boxed{s_{(m-1,m-2,\ldots,1)}\in\mathbb Q[p_1,p_3,p_5,\ldots].}
$$

Finally, the cycle type of an $n$-cycle has one strip of size $n$. A straight diagram is a [border strip](../../../../../rim-hook.md) exactly when its second row has length at most one: otherwise it contains the upper-left $2\times2$ square; conversely the first row with a single-column tail is connected and contains none. These diagrams are exactly the [hook partitions](../../../../../hook-partition.md) $(n-s,1^s)$, of height $s$. There is one strip filling in this case and none otherwise, giving

$$
\boxed{\chi^\lambda(w)=
\begin{cases}
(-1)^s,&\lambda=(n-s,1^s),\\
0,&\text{otherwise}.
\end{cases}}
$$

## ↑ Ancestors (10)

1. [8](../8.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
