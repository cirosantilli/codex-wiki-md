<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $d=\inf\{\|x\|:x\in C\}$. The nonemptiness of $C$ gives $0\le d<\infty$. By [Mazur theorem](../../../../../../../mazur-theorem.md), a norm-closed [convex](../../../../../../../convex-function.md) set is weakly closed. This applies to both $C$ and every closed [norm](../../../../../../../norm.md) ball.

For $n\ge1$, the sets $C_n=C\cap(d+1/n)B_X$ are nonempty by the definition of the [infimum](../../../../../../../infimum.md), weakly closed and nested. They all lie in the [weakly compact set](../../../../../../../weakly-compact-set.md) $(d+1)B_X$, by the [weak compactness characterization of reflexivity](../../../../../../../weak-compactness-characterization-of-reflexivity.md). Hence they have the [finite intersection property](../../../../../../../finite-intersection-property.md), and compactness gives $x_0\in\bigcap_n C_n$. Then $x_0\in C$ and $\|x_0\|\le d+1/n$ for every $n$, so

$$
\boxed{x_0\in C,\qquad\|x_0\|=\min_{x\in C}\|x\|=d.}
$$

This proves the [norm minimizer in a closed convex subset of a reflexive Banach space](../../../../../../../norm-minimizer-in-a-closed-convex-subset-of-a-reflexive-banach-space.md) assertion without assuming sequential weak compactness. It includes $d=0$; uniqueness is not asserted without an additional condition such as strict convexity of the [norm](../../../../../../../norm.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 106](../../../../paper-106-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
