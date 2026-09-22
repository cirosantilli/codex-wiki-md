<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use $\kappa$-completeness in its usual [forcing](../../../../../../forcing-split.md) sense: every decreasing [chain in a partial order](../../../../../../chain-in-a-partial-order.md) of stronger conditions of length less than $\kappa$ has a common stronger bound. Let $\dot f\in M$ and choose $p\in G$ [forcing](../../../../../../forcing-split.md) that it [functions](../../../../../../function-split.md) the ground [ordinal](../../../../../../ordinal.md) $\alpha<\kappa$ into the ground [set](../../../../../../set-split.md) $B$. Below any stronger condition $r$, recursively decide each value of $\dot f$ in order. At a successor step the deciding conditions are dense, and at a limit stage use $\kappa$-completeness. After all $\alpha$ steps take another common bound. The recursion and its choices can be performed in $M$, using ground choice and closure, and it records a [function](../../../../../../function-split.md) $g:\alpha\to B$ in $M$.

Thus below every $r$ stronger than $p$ there is a condition [forcing](../../../../../../forcing-split.md) $\dot f=\check g$ for some ground $g$. The [set](../../../../../../set-split.md) $D$ of such whole-function deciding conditions belongs to $M$ and is dense below $p$. Genericity with $p\in G$ makes $G$ meet $D$: adjoin the conditions incompatible with $p$ to obtain a globally [dense subset of a forcing order](../../../../../../dense-subset-of-a-forcing-order.md), and use directedness to rule out the incompatible alternative. A condition in $G\cap D$ then gives $f=g\in M$.

The reverse inclusion follows because ground [functions](../../../../../../function-split.md) remain [functions](../../../../../../function-split.md) with the same domain and values. Therefore

$$
\boxed{({}^\alpha B)^M=({}^\alpha B)^{M[G]}.}
$$

This [closed forcing adds no short ground-valued sequences](../../../../../../closed-forcing-adds-no-short-ground-valued-sequences.md) argument needs density of complete decisions. A single arbitrarily constructed lower bound need not belong to $G$, and would not by itself prove the claim.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
