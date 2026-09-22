<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix any two [integers](../../../../../integer-split.md) $i,j$. By [Bézout's identity](../../../../../bezout-s-identity.md), there are [integers](../../../../../integer-split.md) $u,v$ with $au-bv=j-i$. Replacing $(u,v)$ by $(u+kb,v+ka)$ leaves this identity unchanged. Choose $k$ large enough that both entries are nonnegative. A path with $u+kb$ upward steps and $v+ka$ downward steps then takes $i$ to $j$, with strictly positive [probability](../../../../../probability.md) $p^{u+kb}q^{v+ka}$. There are no boundary restrictions on this [state space](../../../../../state-space.md).

This applies in both directions, so every pair of states communicates. Hence

$$
\boxed{\text{The Markov chain is irreducible, with sole communicating class }\mathbb Z.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
