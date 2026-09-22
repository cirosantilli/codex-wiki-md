<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [high-energy Roth theorem](../../../../../../high-energy-roth-theorem.md) concludes that, for fixed $\theta>0$, a sufficiently large finite set of [integers](../../../../../../integer.md) with [additive energy](../../../../../../additive-energy.md) at least $\theta|A|^3$ contains a nonconstant three-term [arithmetic progression](../../../../../../arithmetic-progression.md). The size threshold depends on $\theta$, and there is no assumption about the diameter of $A$.

Here is why [additive energy](../../../../../../additive-energy.md) replaces interval [subset density](../../../../../../density-of-a-finite-subset.md). The [Balog-Szemerédi-Gowers theorem](../../../../../../balog-szemeredi-gowers-theorem.md) in the small-[difference set](../../../../../../difference-set.md) form proved in Question 3 supplies $B\subseteq A$ with $|B|\geq c_\theta|A|$ and $|B-B|\leq K_\theta|B|$. The [Petridis minimal-growth lemma](../../../../../../petridis-minimal-growth-lemma.md), the [Ruzsa triangle inequality](../../../../../../ruzsa-triangle-inequality.md), and the [Ruzsa modeling lemma](../../../../../../ruzsa-modelling-lemma.md), all proved there, then give a subset $B'\subseteq B$ of size at least $|B|/16$ and a [Freiman s-isomorphism](../../../../../../freiman-s-isomorphism.md) of order eight onto $D\subseteq\mathbb Z/q\mathbb Z$, where

$$
|B'|\leq q\leq C_\theta|B'|,
\qquad |D|/q\geq C_\theta^{-1}.
$$

Represent $D$ by residues in $\{0,\ldots,q-1\}$. One of the two consecutive half-intervals has [subset density](../../../../../../density-of-a-finite-subset.md) bounded below by a positive constant depending only on $\theta$; their lengths tend to infinity with $|A|$. Apply the [Roth theorem on three-term arithmetic progressions](../../../../../../roth-theorem-on-three-term-arithmetic-progressions.md) proved in part (i) to this interval. The resulting three distinct residues satisfy $d_0+d_2=2d_1$ modulo $q$. The inverse [Freiman homomorphism](../../../../../../freiman-homomorphism.md) preserves that equality and distinctness, so its preimages form a nonconstant three-term [arithmetic progression](../../../../../../arithmetic-progression.md) in $B'$, hence in $A$.

**Large additive energy therefore gives the same three-term progression conclusion after passing to a dense finite model.** A forward reference to the detailed lemmas in Question 3 avoids reproving them here.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
