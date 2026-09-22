<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $[n]^{(r)}$ for the rank-$r$ [uniform layer of the Boolean cube](../../../../../uniform-layer-of-the-boolean-cube.md). For a [uniform set family](../../../../../uniform-set-family.md) $\mathcal F\subseteq[n]^{(r)}$, with $1\leq r\leq n$, let $\partial\mathcal F$ be its [lower shadow](../../../../../lower-shadow.md). The **[Local LYM inequality](../../../../../local-lym-inequality.md)** is

$$
\boxed{\frac{|\partial\mathcal F|}{\binom n{r-1}}\geq\frac{|\mathcal F|}{\binom nr}}.
$$

For its proof, count incidences $(B,A)$ with $A\in\mathcal F$, $B\subset A$, and $|B|=r-1$. Each member of $\mathcal F$ contributes $r$ incidences, while each member of the [lower shadow](../../../../../lower-shadow.md) contributes at most $n-r+1$. Thus $r|\mathcal F|\leq(n-r+1)|\partial\mathcal F|$, which is the displayed bound by the ratio of consecutive [binomial coefficients](../../../../../binomial-coefficient.md). Complementing every set gives the corresponding [upper shadow](../../../../../upper-shadow.md) bound, $|\nabla\mathcal F|/\binom n{r+1}\geq|\mathcal F|/\binom nr$ for $r<n$.

For an [antichain](../../../../../antichain.md) $\mathcal A$ in the [Boolean lattice](../../../../../boolean-lattice.md), the **[LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md)** is

$$
\boxed{\sum_{r=0}^n\frac{|\mathcal A\cap[n]^{(r)}|}{\binom nr}\leq1}.
$$

Here is the proof using the [Local LYM inequality](../../../../../local-lym-inequality.md). Denote the rank-$r$ part by $\mathcal A_r$, and let $\mathcal D_r$ consist of the $r$-sets containing some member of $\mathcal A$ of size at most $r$. These families satisfy

$$
\mathcal D_r=\mathcal A_r\mathbin{\dot\cup}\nabla\mathcal D_{r-1}\quad(1\leq r\leq n),\qquad \mathcal D_0=\mathcal A_0.
$$

The union is disjoint because a member of the [antichain](../../../../../antichain.md) cannot contain a strictly smaller member. Apply the [upper shadow](../../../../../upper-shadow.md) form of the [Local LYM inequality](../../../../../local-lym-inequality.md) to $\mathcal D_{r-1}$:

$$
\frac{|\mathcal D_r|}{\binom nr}\geq\frac{|\mathcal A_r|}{\binom nr}+\frac{|\mathcal D_{r-1}|}{\binom n{r-1}}.
$$

Iterating gives a bound for the entire sum by $|\mathcal D_n|/\binom nn\leq1$. This also covers the empty [antichain](../../../../../antichain.md) and an [antichain](../../../../../antichain.md) containing the empty set.

For the second proof, each [permutation](../../../../../permutation.md) of $[n]$ specifies a [maximal chain in a Boolean lattice](../../../../../maximal-chain-in-a-boolean-lattice.md) by taking its successive prefixes. There are $n!$ such [maximal chains in a Boolean lattice](../../../../../maximal-chain-in-a-boolean-lattice.md), and a fixed $r$-set belongs to $r!(n-r)!$ of them. A [maximal chain in a Boolean lattice](../../../../../maximal-chain-in-a-boolean-lattice.md) meets an [antichain](../../../../../antichain.md) at most once. [Double counting](../../../../../double-counting-proof-technique.md) these incidences therefore gives $\sum_r|\mathcal A_r|r!(n-r)!\leq n!$, exactly the [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md).

The **[Sperner theorem](../../../../../sperner-s-theorem.md)** says that an [antichain](../../../../../antichain.md) in $\mathcal P([n])$ has at most $\binom n{\lfloor n/2\rfloor}$ members; a full middle rank attains this bound. Indeed, every [binomial coefficient](../../../../../binomial-coefficient.md) $\binom nr$ is at most the central one, so the [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md) gives

$$
\frac{|\mathcal A|}{\binom n{\lfloor n/2\rfloor}}\leq\sum_r\frac{|\mathcal A_r|}{\binom nr}\leq1.
$$

Now let $\mathcal F$ be an [intersection-free uniform set family](../../../../../intersection-free-uniform-set-family.md). If it is empty, there is nothing to prove. Fix $X\in\mathcal F$ and consider the traces

$$
\mathcal T=\{X\cap A:A\in\mathcal F\setminus\{X\}\}\subseteq\mathcal P(X).
$$

If $A,B\ne X$ are distinct and $X\cap A\subseteq X\cap B$, then $X\cap A\subseteq B$. This contradicts the defining restriction on the three distinct members $X,A,B$. The intersection has size less than $r$, so it is a proper subset of $B$ even if the printed subset symbol is interpreted strictly. In particular, equal traces are impossible, and the traces form an [antichain](../../../../../antichain.md). Thus $|\mathcal T|=|\mathcal F|-1$. Applying the [Sperner theorem](../../../../../sperner-s-theorem.md) to the $r$-element ground set $X$ proves the [antichain trace bound for intersection-free families](../../../../../antichain-trace-bound-for-intersection-free-families.md)

$$
\boxed{|\mathcal F|\leq1+\binom r{\lfloor r/2\rfloor}}.
$$

The argument also handles $r=0$: a [uniform set family](../../../../../uniform-set-family.md) then has at most one member.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
