<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let the input words be $s,t$, let $L$ be their common length, let $\Sigma$ be the finite [alphabet](../../../../../alphabet.md), and let $D_L$ contain the dictionary words of length $L$. Unequal input lengths immediately make the puzzle impossible because a mutation preserves length. A [word ladder](../../../../../word-ladder.md) [search problem](../../../../../search-problem.md) can use the [state space](../../../../../state-space.md) $S=D_L\cup\{s\}$, with initial state $s$; including $s$ handles an input word not itself in the dictionary.

At word $w$, an action is a position–letter pair $(i,\ell)$ with $1\le i\le L$, $\ell\in\Sigma$ and $\ell\ne w_i$, permitted precisely when replacing $w_i$ by $\ell$ gives $w'\in D_L$. The [search transition model](../../../../../search-transition-model.md) returns that $w'$, and the [goal test](../../../../../goal-test.md) is $w=t$. If $s=t$, the empty sequence is accepted; if $t\notin D_L$ and $s\ne t$, no transition can reach $t$.

Assign each permitted transition cost $1$. A [search node](../../../../../search-node.md) at [search depth](../../../../../search-depth.md) $k$ has

$$
\boxed{g(n)=\sum_{j=1}^{k}1=k.}
$$

Thus minimizing [path cost](../../../../../path-cost.md) is exactly minimizing the number of mutations. [Uniform-cost search](../../../../../uniform-cost-search.md), with repeated states handled by [graph search](../../../../../graph-search.md) and the [goal test](../../../../../goal-test.md) on selection, finds a shortest [word ladder](../../../../../word-ladder.md) if one exists. Because all costs are equal, [breadth-first search](../../../../../breadth-first-search.md) gives the same optimal-length guarantee.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
