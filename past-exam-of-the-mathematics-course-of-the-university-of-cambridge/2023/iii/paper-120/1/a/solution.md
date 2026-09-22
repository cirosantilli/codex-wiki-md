<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Kripke model for intuitionistic propositional logic](../../../../../../kripke-model-for-intuitionistic-propositional-logic.md) is a triple $(W,\leq,V)$ in which $(W,\leq)$ is a [partially ordered set](../../../../../../partially-ordered-set.md) of worlds and $V(p)\subseteq W$ is upward closed for every propositional variable $p$. The [Kripke forcing relation](../../../../../../kripke-forcing-relation.md) is defined recursively by

$$
w\Vdash p\iff w\in V(p),
$$

with the usual clauses for $\top$, $\bot$, conjunction and disjunction, and with

$$
w\Vdash A\to B
\iff
\text{for every }v\geq w,\ v\Vdash A\Longrightarrow v\Vdash B.
$$

The upward closure of the valuation implies [persistence of intuitionistic Kripke forcing](../../../../../../persistence-of-intuitionistic-kripke-forcing.md): if $w\leq v$ and $w\Vdash A$, then $v\Vdash A$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
