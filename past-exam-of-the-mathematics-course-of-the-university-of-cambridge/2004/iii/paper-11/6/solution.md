<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use discrete [Shannon entropy](../../../../../information-entropy.md) with base-two logarithms. The standard facts needed are the [chain rule for information entropy](../../../../../chain-rule-for-information-entropy.md), [conditioning reduces entropy](../../../../../conditioning-reduces-entropy.md), nonnegativity of [conditional entropy](../../../../../conditional-entropy.md), and the fact that a uniform distribution on $M$ outcomes has [Shannon entropy](../../../../../information-entropy.md) $\log_2M$.

Order the coordinates by their indices and put $h_j=H(X_j\mid X_1,\ldots,X_{j-1})\geq0$. Applying the chain rule within a coordinate subset $A$ and then adding the missing earlier conditioning coordinates gives

$$
\begin{aligned}
H(X_A)
&=\sum_{j\in A}H(X_j\mid X_{A\cap[j-1]})\\
&\geq\sum_{j\in A}H(X_j\mid X_{[j-1]})
=\sum_{j\in A}h_j.
\end{aligned}
$$

On summing over the family, coordinate $j$ occurs at least $k$ times. Since each $h_j$ is nonnegative,

$$
\boxed{\sum_{A\in\mathcal A}H(X_A)
\geq k\sum_{j=1}^nh_j=kH(X).}
$$

This proves [Shearer's inequality](../../../../../shearer-s-inequality.md) without any independence assumption on the coordinates. For countable alphabets, apply the finite-valued assertion to refining finite coordinate partitions; the standard monotone approximation of [Shannon entropy](../../../../../information-entropy.md) gives the same result with extended values. [Differential entropy](../../../../../differential-entropy.md) is not the [Shannon entropy](../../../../../information-entropy.md) intended here.

For the [graph](../../../../../graph-split.md) application, let its bipartition be $U,V$, with degrees $a$ on $U$ and $b$ on $V$, where $a,b\geq1$. Choose an [independent set](../../../../../independent-set-graph-theory.md) uniformly from all $i(G)$ such [sets](../../../../../set-split.md), and let $X$ be its vertex-indicator [vector](../../../../../vector.md). Then $H(X)=\log_2i(G)$. For $v\in V$ put $Y_v=X_{N(v)}$ and $q_v=\Pr(Y_v=0)$.

Each vertex of $U$ belongs to exactly $a$ of these neighbourhoods. [Shearer's inequality](../../../../../shearer-s-inequality.md) therefore gives $H(X_U)\leq a^{-1}\sum_{v\in V}H(Y_v)$. Conditional on $X_U$, a vertex of $V$ is forced absent if any neighbor was selected, and otherwise is a free fair binary choice. There are no edges within $V$, and the conditional independent-set distribution is uniform on all these free choices. Hence

$$
H(X_V\mid X_U)=\sum_{v\in V}q_v,
$$

and

$$
H(X)\leq\frac1a\sum_{v\in V}[H(Y_v)+aq_v].
$$

There are $2^b$ possible neighborhood patterns. Give the zero pattern weight $w_0=2^a$ and every other pattern weight one. For its distribution $(p_y)$, concavity of the logarithm, or [Jensen's inequality](../../../../../jensen-s-inequality.md), gives

$$
\begin{aligned}
H(Y_v)+aq_v
&=\sum_{p_y>0}p_y\log_2\frac{w_y}{p_y}\\
&\leq\log_2\sum_{p_y>0}w_y
\leq\log_2(2^a+2^b-1).
\end{aligned}
$$

This establishes the local weighted-entropy estimate rather than just counting neighborhood patterns.

Edge counting gives $a|U|=b|V|$; together with $|U|+|V|=n$, it yields $|V|/a=n/(a+b)$. Exponentiating the [Shannon entropy](../../../../../information-entropy.md) estimate proves the [independent-set bound for biregular graphs](../../../../../independent-set-bound-for-biregular-graphs.md):

$$
\boxed{i(G)\leq(2^a+2^b-1)^{n/(a+b)}.}
$$

The complete bipartite [graph](../../../../../graph-split.md) $K_{b,a}$ has exactly $2^a+2^b-1$ [independent sets](../../../../../independent-set-graph-theory.md), since one chooses a subset of one side and subtracts the double-counted empty [set](../../../../../set-split.md). Disjoint unions of such components attain equality. If exactly one degree parameter is zero, edge counting forces the [graph](../../../../../graph-split.md) to be edgeless and the displayed bound equals $2^n$, so it remains valid. If $a=b=0$, the denominator is undefined; the edgeless [graph](../../../../../graph-split.md) has exactly $2^n$ [independent sets](../../../../../independent-set-graph-theory.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
