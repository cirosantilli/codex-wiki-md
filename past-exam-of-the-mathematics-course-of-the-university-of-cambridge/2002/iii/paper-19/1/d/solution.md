<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**True with the stated Conway normalization.** Fix $t^{1/2}=i$ at $t=-1$. The [Jones polynomial skein relation](../../../../../../jones-polynomial-skein-relation.md) becomes

$$
V_{L_+}(-1)-V_{L_-}(-1)=-2iV_{L_0}(-1).
$$

The [Conway polynomial](../../../../../../conway-polynomial-knot-theory.md) satisfies $\nabla_{L_+}(z)-\nabla_{L_-}(z)=z\nabla_{L_0}(z)$. Put $W_L=(-1)^{\ell(L)-1}\nabla_L(2i)$. An [oriented smoothing](../../../../../../oriented-smoothing.md) changes the number of components by one, so these quantities satisfy precisely $W_{L_+}-W_{L_-}=-2iW_{L_0}$. Both $W$ and $V(-1)$ are one on the [unknot](../../../../../../unknot.md) and zero on every multi-component [unlink](../../../../../../unlink.md): for $V$, the split-union factor vanishes at this substitution.

These [skein relations](../../../../../../skein-relation.md) and [unlink](../../../../../../unlink.md) values determine the invariants uniquely. Switching a first undesired crossing gives a diagram closer to a descending diagram, while the smoothing term has fewer crossings; induction first on crossing count and then on undesired crossings reduces everything to [unlinks](../../../../../../unlink.md). Thus $W_L=V_L(-1)$. For a [knot](../../../../../../knot.md) there is one component and the [Conway-normalized Alexander polynomial](../../../../../../conway-normalized-alexander-polynomial.md) gives

$$
\boxed{V_K(-1)=\nabla_K(2i)=\Delta_K(-1).}
$$

This is the [signed Jones evaluation at minus one](../../../../../../signed-jones-evaluation-at-minus-one.md). Replacing $\Delta_K$ by an arbitrary [Laurent unit](../../../../../../unit-of-a-laurent-polynomial-ring.md) multiple would destroy the signed conclusion.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
