<h1 id="b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [dependency digraph](../../../../../independence-digraph-of-events.md) has [vertices](../../../../../vertex-graph-theory.md) $1,\ldots,n$ and no loops. For each $i$, the [event](../../../../../event.md) $A_i$ must be [independent](../../../../../independent-random-variables.md) of the [sigma-algebra](../../../../../sigma-algebra.md) generated jointly by all $A_j$ with $j\neq i$ for which there is no [edge](../../../../../edge-of-a-graph.md) $i\to j$. Joint [independence](../../../../../independent-random-variables.md) from that collection is required; [pairwise independence](../../../../../pairwise-independent-events.md) alone does not suffice.

Write $\Gamma^+(i)$ for the outneighbours of $i$, and $B_S=\bigcap_{j\in S}A_j^c$. We prove by [induction](../../../../../mathematical-induction.md) on $|S|$ that $B_S$ has positive [probability](../../../../../probability.md) and, when $i\notin S$,

$$
\mathbb P(A_i\mid B_S)\leq x_i.
$$

For $S=\varnothing$, the asserted conditional bound follows from the hypothesis, since its product factors are at most one. For the [induction](../../../../../mathematical-induction.md) step, positivity for a [set](../../../../../set-split.md) of size $r$ follows by writing its avoidance [probability](../../../../../probability.md) as a chain product: all preceding conditioning [sets](../../../../../set-split.md) have size below $r$, so each factor is at least $1-x_j>0$.

Now take $|S|=r$, split $S_1=S\cap\Gamma^+(i)$ and $S_2=S\setminus\Gamma^+(i)$, and condition first on $B_{S_2}$. [Independence](../../../../../independent-random-variables.md) gives $\mathbb P(A_i\mid B_{S_2})=\mathbb P(A_i)$. Moreover, order the elements of $S_1$ and use the inductive conditional bounds on the successive avoidance factors. Their conditioning [sets](../../../../../set-split.md) have size at most $r-1$, so

$$
\mathbb P(B_{S_1}\mid B_{S_2})\geq\prod_{j\in S_1}(1-x_j).
$$

This remains true when $S_1$ is empty, with both sides one. Therefore

$$
\begin{aligned}
\mathbb P(A_i\mid B_S)
&=\frac{\mathbb P(A_i\cap B_{S_1}\mid B_{S_2})}{\mathbb P(B_{S_1}\mid B_{S_2})}\\
&\leq\frac{\mathbb P(A_i)}{\prod_{j\in S_1}(1-x_j)}\\
&\leq x_i\prod_{j\in\Gamma^+(i)\setminus S_1}(1-x_j)\leq x_i.
\end{aligned}
$$

The [induction](../../../../../mathematical-induction.md) is complete. Finally expand the [probability](../../../../../probability.md) of avoiding all [events](../../../../../event.md) in the order $1,\ldots,n$:

$$
\boxed{\mathbb P\left(\bigcap_{i=1}^nA_i^c\right)
=\prod_{i=1}^n\left(1-\mathbb P\left(A_i\,\middle|\,\bigcap_{j<i}A_j^c\right)\right)
\geq\prod_{i=1}^n(1-x_i)>0.}
$$

This proves the asymmetric [Lovász local lemma](../../../../../lovasz-local-lemma.md), including the positivity needed to make every conditioning step legitimate.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
