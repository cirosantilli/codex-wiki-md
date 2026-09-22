<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The norm comparison in [bounded distortion of a Banach space](../../../../../bounded-distortion-of-a-banach-space.md) is understood up to a positive rescaling of the new norm. Thus, after replacing $D$ by $D^2$ if one's convention uses symmetric comparison constants, we may use the following form: for every equivalent norm $q$ on a [block subspace](../../../../../block-subspace.md), a further block subspace $Z$ and a number $a>0$ satisfy

$$
a\|z\|\leq q(z)\leq aD\|z\|\qquad(z\in Z).
$$

The number $a$ may depend on the norm and the subspace; $D$ is fixed. Without this rescaling convention the premise would be impossible, since arbitrarily large scalar multiples of the original norm are equivalent norms. We prove the substantive, scale-invariant assertion for an infinite [Schauder basis](../../../../../schauder-basis.md).

Let $K$ be the [basis constant](../../../../../basis-constant.md) of the original basis. Every [block sequence](../../../../../block-sequence.md) has basis constant at most $K$, so its initial, tail and finite interval [projections](../../../../../projection-linear-algebra.md) have norms at most $K$, $1+K$ and $2K$, respectively. We shall construct increasingly complicated finite unconditional configurations while keeping their unconditional constant fixed at $C=2D$.

First construct the [Maurey hierarchy of finite sets](../../../../../maurey-hierarchy-of-finite-sets.md). Write $\mathcal M_0=\{\varnothing\}$, and define

$$
\mathcal M_{\alpha+1}=\mathcal M_\alpha\cup\bigl\{\{n\}\cup F:F\in\mathcal M_\alpha,\ n<\min F\bigr\},
$$

where prepending to the empty set is permitted. For each nonzero countable limit [ordinal](../../../../../ordinal.md) $\lambda$, fix positive ordinals $\lambda_j\uparrow\lambda$ and put

$$
\mathcal M_\lambda=\{\varnothing\}\cup\bigl\{F\in\mathcal M_{\lambda_j}:j\leq\min F\text{ for some }j\bigr\}.
$$

Induction shows that every family is hereditary and spreading: subsets remain in the family, and increasing any of the coordinates preserves membership. Every nonzero stage contains all singletons. These families are also well-founded as extension trees. At a successor stage, an infinite branch would yield an infinite branch at the previous stage after deleting its first integer. At a limit stage, a hypothetical branch with first integer $m$ has every initial segment in the finite union $\bigcup_{j\leq m}\mathcal M_{\lambda_j}$. One family then contains arbitrarily long initial segments, and heredity would give it an infinite branch.

For every infinite set $L$, the extension tree $\mathcal M_\alpha\cap[L]^{<\infty}$ has empty-root [rank of a well-founded tree](../../../../../rank-of-a-well-founded-tree.md) at least $\alpha$. Here is the induction proving this lower bound. At a successor stage fix $n\in L$; the tree above the node $\{n\}$ contains a copy of $\mathcal M_\alpha$ restricted to the infinite tail of $L$ after $n$, and hence has rank at least $\alpha$. The root therefore has rank at least $\alpha+1$. At a limit stage, for every $j$ the restriction of $\mathcal M_{\lambda_j}$ to a sufficiently late infinite tail of $L$ is contained in $\mathcal M_\lambda$. The root rank is consequently at least $\sup_j\lambda_j=\lambda$.

The crucial elementary estimate concerns [signed interval projection norms](../../../../../signed-interval-projection-norm.md). Given a hereditary family $\mathcal F$ containing all singletons and a basis $(w_i)$, define on finitely supported vectors

$$
q_{\mathcal F}^{(w)}(x)=\sup\left\{\left\|\sum_{i=1}^r\varepsilon_iP_{E_i}^{(w)}x\right\|:E_1<\cdots<E_r\text{ finite intervals},\ (\min E_i)_{i=1}^r\in\mathcal F,\ \varepsilon_i\in\{-1,1\}\right\}.
$$

Choosing one interval containing the support gives $q_{\mathcal F}^{(w)}(x)\geq\|x\|$. Whenever this supremum is bounded by a multiple of $\|x\|$, it extends to a norm on the closed span giving [equivalent norms](../../../../../equivalent-norms.md) with the original norm.

If $S=\sum_i\varepsilon_iP_{E_i}$ is one of the admitted signed interval projections, then

$$
q_{\mathcal F}^{(w)}(Sx)\leq2q_{\mathcal F}^{(w)}(x).
$$

To prove this, test $Sx$ with another admitted operator $R=\sum_j\delta_jP_{F_j}$. The composition is the signed sum of projections onto the nonempty intervals $E_i\cap F_j$. Colour each intersection according to which of $E_i,F_j$ supplies its left endpoint, breaking ties in favour of $E_i$. In the first colour the list of minima is a subset of $(\min E_i)$, with no repetitions; in the second it is a subset of $(\min F_j)$. Both lists belong to $\mathcal F$ by heredity. Each colour therefore contributes an admitted signed interval projection, and the [triangle inequality](../../../../../triangle-inequality.md) gives $\|RSx\|\leq2q_{\mathcal F}^{(w)}(x)$. Taking the supremum over $R$ proves the estimate.

Now suppose $q_{\mathcal F}^{(w)}$ is an equivalent norm on a [block subspace](../../../../../block-subspace.md) $W$. Apply bounded distortion to obtain a further block basis $(z_i)$ spanning $Z$, with $a\|z\|\leq q_{\mathcal F}^{(w)}(z)\leq aD\|z\|$. A signed interval projection relative to $(z_i)$, with an admissible list of minima, is the restriction of an admitted signed interval projection relative to $(w_i)$. Indeed, replace each interval of block indices by the interval from the first to the last original coordinate of its blocks; its minimum only increases, so the spreading property preserves admissibility. The elementary estimate and the norm comparison therefore give

$$
\|Sz\|\leq a^{-1}q_{\mathcal F}^{(w)}(Sz)\leq2a^{-1}q_{\mathcal F}^{(w)}(z)\leq2D\|z\|.
$$

In particular $q_{\mathcal F}^{(z)}\leq C\|\cdot\|$, with the same $C=2D$ for every family to which we apply this procedure.

We prove by [transfinite induction](../../../../../transfinite-induction.md) that, in every block subspace and for every $1\leq\alpha<\omega_1$, there is a normalized block basis $(z_i)$ for which

$$
q_{\mathcal M_\alpha}^{(z)}(x)\leq C\|x\|.
$$

For $\alpha=1$ only one interval is permitted, so the initial [signed interval projection norm](../../../../../signed-interval-projection-norm.md) is bounded by $2K\|x\|$. Apply the preceding renorming procedure.

For a successor stage, first choose $(w_i)$ satisfying the induction hypothesis for $\mathcal M_\alpha$. Delete the first interval from any $\mathcal M_{\alpha+1}$-admissible family. The remaining minima lie in $\mathcal M_\alpha$, so

$$
q_{\mathcal M_{\alpha+1}}^{(w)}(x)\leq(2K+C)\|x\|.
$$

This is an equivalent norm. The renorming procedure produces a further block basis with the constant reset to $C$.

At a limit stage $\lambda$, choose decreasing block subspaces $W_j$, each with a block basis satisfying the induction hypothesis for $\mathcal M_{\lambda_j}$. Choose successive normalized $z_j\in W_j$. Make each $z_j$ sufficiently far out that its first coordinate in the basis of every $W_k$, $k\leq j$, is at least $j$; only finitely many restrictions are imposed at each choice. An admissible interval family for $\mathcal M_\lambda$ belongs to $\mathcal M_{\lambda_j}$ for some $j\leq\min E_1$. All blocks on which it acts lie in the tail $[z_i:i\geq j]\subset W_j$. Transferring its intervals to the basis of $W_j$ increases their minima, so the induction hypothesis gives

$$
\left\|\sum_i\varepsilon_iP_{E_i}^{(z)}x\right\|\leq C\|P_{[j,\infty)}^{(z)}x\|\leq C(1+K)\|x\|.
$$

Thus $q_{\mathcal M_\lambda}^{(z)}$ is again an equivalent norm, and one more application of bounded distortion resets its bound to $C$. This completes the transfinite induction. The tail-projection factor in this step is important; the diagonal tail need not have the same norm as the original vector.

Finally let $T_C(X)$ be the tree of finite normalized sequences $(x_1,\ldots,x_n)$ satisfying

$$
\left\|\sum_{i=1}^n\varepsilon_i a_ix_i\right\|\leq C\left\|\sum_{i=1}^na_ix_i\right\|
$$

for all scalars and all signs. Each finite level is closed in the corresponding power of the unit sphere, since the norm inequalities are closed conditions. The unit sphere of the separable [Banach space](../../../../../banach-space-split.md) $X$ is a [Polish space](../../../../../polish-space.md). An infinite branch is an [unconditional basic sequence](../../../../../unconditional-basic-sequence.md): sign changes give coordinate projections with norm at most $(1+C)/2$, imply linear independence, and give uniformly bounded initial projections, hence the basis property on the closed span. These projection bounds also give unconditional convergence, including over complex scalars.

For each countable $\alpha$, the block basis constructed above maps the extension tree $\mathcal M_\alpha$ into $T_C(X)$ by $\{i_1<\cdots<i_r\}\mapsto(z_{i_1},\ldots,z_{i_r})$. To check the sign inequality, use the admissible singleton intervals $\{i_1\},\ldots,\{i_r\}$ on the vector $\sum a_kz_{i_k}$. Thus the [unconditional tree index](../../../../../unconditional-tree-index.md) is at least $\alpha$ for every countable ordinal. If $T_C(X)$ were well-founded, the closed-tree result would give it countable height, contradicting these lower bounds. It has an infinite branch. **Therefore $X$ contains an unconditional basic sequence.**

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
