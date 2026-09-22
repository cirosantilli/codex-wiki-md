<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Ignore the fox and obstacles when estimating the remaining number of rabbit moves. Define the [heuristic function](../../../../../heuristic-function.md)

$$
\boxed{h(r,f)=\min_{e\in H}\bigl(|r_1-e_1|+|r_2-e_2|\bigr).}
$$

This is [Manhattan distance](../../../../../manhattan-distance.md) to the nearest exit, a [relaxation heuristic](../../../../../relaxation-heuristic.md). Assume at least one exit; with none the instance is immediately unsolvable. The estimate is generally nonconstant and is not the perfect escape cost: obstacles can force detours, while pursuit can make an apparently nearby exit unreachable.

To prove it is a [consistent heuristic](../../../../../consistent-heuristic.md), consider a surviving one-round transition from $(r,f)$ to $(r',f')$. Let $e'$ attain the minimum defining $h(r',f')$. The [triangle inequality](../../../../../triangle-inequality.md) for [Manhattan distance](../../../../../manhattan-distance.md) and the rabbit's move bound give

$$
h(r,f)\le d_1(r,e')\le d_1(r,r')+d_1(r',e')
\le 1+h(r',f').
$$

Every successful terminal state has $h=0$. This proves consistency with unit round costs; summing the inequality along any successful route also proves that it is an [admissible heuristic](../../../../../admissible-heuristic.md). Failed transitions need no successor estimate because they are discarded.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
