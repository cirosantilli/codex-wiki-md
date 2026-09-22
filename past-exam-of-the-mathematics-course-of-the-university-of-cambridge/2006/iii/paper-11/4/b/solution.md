<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $K\geq1$, define the normalized $\ell^1$ tree

$$
T_K(X)=\left\{(x_1,\ldots,x_n)\in S_X^{<\omega}:\frac1K\sum|a_i|\leq\left\|\sum a_ix_i\right\|\leq\sum|a_i|\text{ for all scalars }a_i\right\}.
$$

The upper bound follows from normalization. This is a closed tree: it suffices to impose the lower inequalities for a countable dense set of scalar tuples. The [Bourgain l1-index](../../../../../../bourgain-l1-index.md) is

$$
\boxed{I_1(X)=\sup_{K\in\mathbb N}o(T_K(X)),}
$$

where $o$ is its well-founded tree order, and the index is $\omega_1$ if a tree is ill-founded. An infinite branch is exactly a sequence equivalent to the unit vector basis of $\ell^1$.

If $X$ is separable and contains no $\ell^1$, its unit sphere is Polish and every $T_K(X)$ is closed and well-founded. Part (a) makes each order countable, and their countable supremum is countable. In particular every separable [reflexive Banach space](../../../../../../reflexive-banach-space.md) has countable index, since its closed subspaces are reflexive whereas $\ell^1$ is not.

We now construct separable reflexive spaces with arbitrarily high index. Take any countable well-founded rooted tree $T$. Recursively, at each node $t$, define

$$
X_t=\mathbb R\oplus_1\left(\bigoplus_{s\text{ an immediate child of }t}X_s\right)_{\ell^2}.
$$

At a terminal node this is just $\mathbb R$. The recursion is legitimate by well-foundedness. Each $X_t$ is separable and reflexive: a countable $\ell^2$ sum of separable reflexive spaces is separable and reflexive, and adjoining one dimension in a finite direct sum preserves reflexivity. Let $X_T$ be the root space, and let $e_t$ be the unit vector at each node coordinate.

Along every finite branch $t_1\prec\cdots\prec t_n$, the recursive norm is exactly

$$
\left\|\sum_{i=1}^na_ie_{t_i}\right\|=\sum_{i=1}^n|a_i|.
$$

Indeed, at every step only one child component is occupied, so its $\ell^2$ norm equals that component's norm, while the node coordinate adds by the $\ell^1$ sum. Thus $T$ embeds by extension into $T_1(X_T)$, and its rank is a lower bound for the index, up to the harmless empty-root convention. Countable well-founded trees have arbitrarily high countable ranks: add a root for a successor stage and attach countably many trees of cofinal ranks at a limit stage.

Suppose now a separable reflexive space $U$ were universal. Put $\beta=I_1(U)<\omega_1$ and choose $T$ of height larger than $\beta$. An isomorphic embedding $J:X_T\to U$ has bounds $c\|x\|\leq\|Jx\|\leq C\|x\|$. The normalized images $Je_t/\|Je_t\|$ along each branch satisfy the lower $\ell^1$ estimate $c/C$, so the tree embeds into $T_K(U)$ for some integer $K\geq C/c$. It would have order greater than $\beta$, contradicting its definition. Therefore **no separable reflexive Banach space is universal for all separable reflexive Banach spaces**. The embedding constant need not be uniform across spaces; the supremum over all $K$ handles this.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
