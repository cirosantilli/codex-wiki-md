<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a finite [group action](../../../../../group-action.md) $G\curvearrowright X$, [Burnside's lemma](../../../../../burnside-s-lemma.md) states

$$
\boxed{|X/G|=\frac1{|G|}\sum_{g\in G}|\operatorname{Fix}_X(g)|.}
$$

Count pairs $(g,x)$ with $gx=x$ in two ways. Counting first by $g$ gives the displayed sum. Counting first by $x$ gives $\sum_x|G_x|$. For an orbit $\mathcal O$, the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) gives $|\mathcal O||G_x|=|G|$, so each orbit contributes exactly $|G|$. Division proves the formula.

Use colors $1,\ldots,m$, with variables $x_1,\ldots,x_m$, on the underlying finite set $S$. The weight of a coloring $f:S\to\{1,\ldots,m\}$ is $w(f)=\prod_{s\in S}x_{f(s)}$. It is constant on each coloring orbit. The [pattern inventory](../../../../../pattern-inventory.md) is $F_G(x)=\sum_{\mathcal O}w(\mathcal O)$, one weight for each orbit, including its multiplicity when different orbits have the same content.

If $c_r(g)$ is the number of length-$r$ cycles of $g$ on $S$, define the [cycle index](../../../../../cycle-index.md)

$$
Z_G(t_1,t_2,\ldots)=\frac1{|G|}\sum_{g\in G}\prod_rt_r^{c_r(g)}.
$$

In the symmetric-function cycle-indicator convention, write $Z_G(x)$ for its substitution $t_r=p_r(x)=\sum_{i=1}^m x_i^r$. A fixed coloring must be constant on every cycle of $g$. Coloring one length-$r$ cycle therefore has weight sum $p_r(x)$, independently of other cycles. The [weighted Burnside lemma](../../../../../weighted-burnside-lemma.md), proved by exactly the same orbit-stabilizer double count with weights, yields

$$
\boxed{F_G(x)=\frac1{|G|}\sum_{g\in G}\prod_rp_r(x)^{c_r(g)}=Z_G(x).}
$$

This defines both sides in the same alphabet; the raw cycle index in the independent variables $t_r$ is specialized before comparison. The identity holds for all finite $m$ and hence stably for arbitrarily many colors.

For the last assertion, the [permutation character](../../../../../permutation-character.md) on $T$ satisfies $\chi(g)=|\operatorname{Fix}_T(g)|$. A pair $(s,t)$ is fixed in the diagonal action on $T\times T$ exactly when both components are fixed. Therefore

$$
|\operatorname{Fix}_{T\times T}(g)|=\chi(g)^2.
$$

The character is real, so its [character inner product](../../../../../character-inner-product.md) with itself and another application of [Burnside's lemma](../../../../../burnside-s-lemma.md) give

$$
\boxed{\langle\chi,\chi\rangle
=\frac1{|G|}\sum_g\chi(g)^2
=|(T\times T)/G|=\operatorname{rank}(G\curvearrowright T).}
$$

This is the [rank of a permutation action](../../../../../rank-of-a-permutation-action.md) formula, and in fact does not require transitivity. If the action is transitive and $|T|\ge2$, the diagonal is one orbit; rank two means exactly one further orbit on distinct ordered pairs, which is double transitivity.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
