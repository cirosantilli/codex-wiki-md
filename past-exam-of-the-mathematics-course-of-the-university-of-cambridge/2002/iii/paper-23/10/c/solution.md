<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We use the finite-structure convention of Section B. Express that $<$ is a strict [linear order](../../../../../../linear-order.md) by irreflexivity, transitivity and comparability of distinct points. Express that $E$ is an [equivalence relation](../../../../../../equivalence-relation.md) by reflexivity, symmetry and transitivity. All these assertions use at most the three variable names $x,y,z$.

In a finite linearly ordered structure, every [equivalence class](../../../../../../equivalence-class.md) has a unique least element. The two-variable formula

$$
\operatorname{Rep}(x)=\forall y\,[y<x\longrightarrow\neg E(y,x)]
$$

selects exactly those least elements. Apply part (b) to this formula, using $k=3$, to obtain $\operatorname{Rep}_n\in L^3$ saying that at least $n$ representatives exist. The required sentence is

$$
\boxed{\eta_n=\operatorname{Lin}(<)\land\operatorname{Eq}(E)\land\operatorname{Rep}_n.}
$$

This gives the [least representatives of finite equivalence classes](../../../../../../least-representatives-of-finite-equivalence-classes.md) construction. Under the two structural axioms, counting representatives is exactly counting [equivalence classes](../../../../../../equivalence-class.md).

Finiteness is essential to the assertion as written in this section. If it were interpreted as applying to all infinite structures, the general claim would fail, not merely this choice of representatives. Partition the rational order into three dense classes, or into four dense classes, and let $E$ mean belonging to the same class. In the three-pebble version of the [Ehrenfeucht-Fraïssé game](../../../../../../ehrenfeucht-fraisse-game.md), the duplicator can play indefinitely between these structures: after one pebble is moved, at most two old classes remain represented; a new point can be placed in the required interval in its corresponding old class, or in a class different from both. Density makes every required placement possible in either structure. Thus the structures agree on all $L^3$ sentences although one has three classes and the other four. The finite reading of the printed request is therefore necessary for $n=4$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10](../../10.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
