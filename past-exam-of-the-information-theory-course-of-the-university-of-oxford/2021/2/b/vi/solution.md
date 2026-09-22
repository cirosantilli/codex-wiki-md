<h1 id="2/b/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Assume a [full-support finite distribution](../../../../../full-support-probability-distribution-on-a-finite-alphabet.md). The preceding structural arguments show that every internal [vertex](../../../../../vertex-graph-theory.md) has three [tree children](../../../../../child-in-a-rooted-tree.md), except possibly one [tree parent](../../../../../parent-in-a-rooted-tree.md) at depth $L-1$ with two [tree children](../../../../../child-in-a-rooted-tree.md). Let $N_3$ and $N_2$ count these two kinds of internal [vertex](../../../../../vertex-graph-theory.md). Part iv gives $N_2\in\{0,1\}$; no [vertex](../../../../../vertex-graph-theory.md) has one [tree child](../../../../../child-in-a-rooted-tree.md).

A finite [rooted tree](../../../../../rooted-tree.md) with $m$ [tree leaves](../../../../../leaf-of-a-tree.md) has $m+N_2+N_3-1$ [edges](../../../../../edge-of-a-graph.md), while counting outgoing [edges](../../../../../edge-of-a-graph.md) gives $2N_2+3N_3$. Equating the counts yields

$$
m=1+N_2+2N_3.
$$

For an [odd integer](../../../../../odd-integer.md) $m$, the right side forces $N_2$ to be an [even integer](../../../../../even-number.md). Since it is at most one, **$N_2=0$**. Thus no deepest pair has only two [sibling codewords](../../../../../sibling-leaves-in-a-code-tree.md), and the optimal [code tree](../../../../../prefix-tree-of-a-code.md) is a [full ternary tree](../../../../../full-ternary-tree.md). This leaf-count identity also directly proves that a [full ternary tree](../../../../../full-ternary-tree.md) has an [odd number](../../../../../odd-number.md) of [tree leaves](../../../../../leaf-of-a-tree.md).

Again the unrestricted zero-weight version is false: $(0,10,11)$ is an optimal [prefix code](../../../../../prefix-code.md) for $p=(1,0,0)$, with [odd integer](../../../../../odd-integer.md) $m=3$, but its two deepest [tree leaves](../../../../../leaf-of-a-tree.md) form a two-sibling pair. There is no contradiction with the proof because its [tree root](../../../../../root-of-a-tree.md) has only two [tree children](../../../../../child-in-a-rooted-tree.md), which the [full-support finite distribution](../../../../../full-support-probability-distribution-on-a-finite-alphabet.md) assumption would forbid above the deepest level.

## ↑ Ancestors (13)

1. [Vi](../vi.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the information theory course of the University of Oxford](../../../../split.md)
6. [Information theory course of the University of Oxford](../../../../../information-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
