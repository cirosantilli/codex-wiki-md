# Coordinate-splitting proof of the BK inequality

↑ **Parent:** [Van den Berg-Kesten inequality](van-den-berg-kesten-inequality.md)

For [increasing events](increasing-event.md) $A,B$ under a finite [Bernoulli distribution](bernoulli-distribution.md) [product measure](product-measure.md), first assume all parameters are at most $1/2$. Write $A_0\subseteq A_1$ and $B_0\subseteq B_1$ for last-coordinate sections. The zero-section of their [disjoint occurrence of increasing events](disjoint-occurrence-of-increasing-events.md) is $A_0\square B_0$; its one-section is $(A_1\square B_0)\cup(A_0\square B_1)$. The intersection in this union contains $A_0\square B_0$. If $a_i=\mathbb P(A_i)$, $b_i=\mathbb P(B_i)$ and the last parameter is $p\leq1/2$, [mathematical induction](mathematical-induction.md) bounds disjoint occurrence by $(1-2p)a_0b_0+p a_1b_0+p a_0b_1$. The product of the two marginal [probabilities](probability.md) exceeds this bound by $p^2(a_1-a_0)(b_1-b_0)\geq0$. For a larger parameter $p_i<1$, replace that coordinate by the [logical disjunction](logical-disjunction.md) of $m_i$ [independent](independent-random-variables.md) bits with parameter $1-(1-p_i)^{1/m_i}\leq1/2$. Disjoint original witnesses lift to disjoint bit witnesses. Apply the small-parameter inequality and then pass to degenerate parameters by continuity.

## ↑ Ancestors (8)

1. [Van den Berg-Kesten inequality](van-den-berg-kesten-inequality.md)
2. [Bond percolation](bond-percolation-split.md)
3. [Percolation theory](percolation-theory.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
