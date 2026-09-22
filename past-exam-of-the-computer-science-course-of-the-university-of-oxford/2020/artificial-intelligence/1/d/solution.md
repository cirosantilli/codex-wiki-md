<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**The proposed [Hamming distance](../../../../../hamming-distance.md) is both an [admissible heuristic](../../../../../admissible-heuristic.md) and a [consistent heuristic](../../../../../consistent-heuristic.md).** Write

$$
h(w)=|\{i:w_i\ne t_i\}|.
$$

Every position differing from the target must change at least once along any successful [word ladder](../../../../../word-ladder.md). One mutation changes only one position, so every solution from $w$ has at least $h(w)$ steps. This proves $h(w)\le h^*(w)$, including an unreachable target with $h^*(w)=\infty$. Dictionary restrictions may force extra changes, but cannot remove that lower bound.

Adjacent words differ in one position, so their [Hamming distances](../../../../../hamming-distance.md) to $t$ differ by at most one. Since every transition costs one,

$$
h(w)\le1+h(w'),\qquad h(t)=0.
$$

These are exactly the [consistent heuristic](../../../../../consistent-heuristic.md) conditions. Equivalently, allowing all length-$L$ words gives a [relaxation heuristic](../../../../../relaxation-heuristic.md) whose exact distance is the [Hamming distance](../../../../../hamming-distance.md); restoring the dictionary can only increase the minimum required number of steps.

## ↑ Ancestors (11)

1. [D](../d.md)
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
