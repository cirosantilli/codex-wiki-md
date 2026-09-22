<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Yes: $h_1(R)=|R|$ is an [admissible heuristic](../../../../../admissible-heuristic.md).** One application of the [resolution inference rule](../../../../../resolution-inference-rule.md) removes just one current negative [Boolean literal](../../../../../boolean-literal.md). It may add other negative [Boolean literals](../../../../../boolean-literal.md), and some of those may already occur, but it cannot remove any other current obligation. Consequently

$$
|R'|\ge |R|-1.
$$

If $\ell$ actions lead from $R$ to $\varnothing$, applying this inequality at every step gives $0\ge |R|-\ell$. Thus

$$
\boxed{h_1(R)=|R|\le\ell,\qquad h_1(R)\le h^*(R).}
$$

It is also a [consistent heuristic](../../../../../consistent-heuristic.md), since $h_1(R)\le1+h_1(R')$ and $h_1(\varnothing)=0$. In particular, merging duplicate obligations cannot invalidate the lower bound: removing several duplicates from the representation never counts as removing several distinct members of a [set](../../../../../set-split.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Intelligent systems](../../../intelligent-systems-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
