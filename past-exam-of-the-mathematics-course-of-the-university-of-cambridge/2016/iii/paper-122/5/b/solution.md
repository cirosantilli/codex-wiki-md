<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A useful [comodule natural transformation formula](../../../../../../comodule-natural-transformation-formula.md) determines $\beta$ from a single [linear functional](../../../../../../linear-functional.md). Define

$$
\alpha=\varepsilon_H\beta_H:H\to k,
$$

using the regular right [comodule](../../../../../../comodule.md) $H$. For any [vector space](../../../../../../vector-space-split.md) $V$, the cofree right [comodule](../../../../../../comodule.md) $V\otimes H$ has coaction $1_V\otimes\Delta$. [Naturality](../../../../../../naturality.md) with respect to all maps $h\mapsto v\otimes h$ gives

$$
\beta_{V\otimes H}=1_V\otimes\beta_H.
$$

The coaction $\rho_M:M\to M\otimes H$ is itself a morphism of right [comodules](../../../../../../comodule.md). Its [naturality](../../../../../../naturality.md) equation, followed by $1_M\otimes\varepsilon_H$, therefore gives

$$
\boxed{\beta_M(u)=\sum u_{(0)}\alpha(u_{(1)}).}
$$

This derivation works for all [comodules](../../../../../../comodule.md), not merely finite-dimensional ones.

The monoidal equation $\beta_{M\otimes N}=\beta_M\otimes\beta_N$, evaluated on the two regular [comodules](../../../../../../comodule.md) and followed by their [counits](../../../../../../counit.md), implies

$$
\alpha(ab)=\alpha(a)\alpha(b).
$$

The unit equation gives $\alpha(1)=1$. Thus $\alpha$ is a unital [algebra homomorphism over a field](../../../../../../algebra-homomorphism-over-a-field.md) $H\to k$. In addition, the $K$-colinearity of $\beta_H$ gives the useful intertwining relation

$$
\sum g(h_{(1)})\alpha(h_{(2)})=\sum\alpha(h_{(1)})f(h_{(2)}).
$$

This fixes the orientation of $\alpha$ relative to $f,g$.

For the [convolution product for coalgebra maps](../../../../../../convolution-product-for-coalgebra-maps.md), define $\alpha^{-1}=\alpha S$. Multiplicativity of $\alpha$ and the two [antipode](../../../../../../antipode.md) identities show

$$
\sum\alpha(h_{(1)})\alpha(S(h_{(2)}))=\varepsilon(h),\qquad\sum\alpha(S(h_{(1)}))\alpha(h_{(2)})=\varepsilon(h).
$$

Consequently

$$
\boxed{\beta_M^{-1}(u)=\sum u_{(0)}\alpha(S(u_{(1)})).}
$$

Coassociativity and the two convolution identities verify both composites directly. Since $\beta_M$ was a $K$-comodule morphism, its linear inverse is also a $K$-comodule morphism. Inverting the [naturality](../../../../../../naturality.md) and monoidal equations shows that the inverses form a monoidal [natural transformation](../../../../../../natural-transformation.md) $g_*\Rightarrow f_*$. **Every such monoidal transformation is therefore invertible**, without requiring a bijective antipode.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
