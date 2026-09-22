<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [diffeomorphism](../../../../../../diffeomorphism.md), the differential and its inverse preserve the natural pairing of a [vector](../../../../../../vector.md) with a [covector](../../../../../../covector.md). Consequently the [mixed tensor pullback](../../../../../../pullback-of-a-mixed-tensor-by-a-diffeomorphism.md) commutes with every [tensor contraction](../../../../../../tensor-contraction.md) $C$:

$$
\phi_s^*(CT)=C(\phi_s^*T).
$$

Differentiating at zero gives $\mathcal L_X(CT)=C(\mathcal L_XT)$. The [mixed tensor pullback](../../../../../../pullback-of-a-mixed-tensor-by-a-diffeomorphism.md) also preserves [tensor products](../../../../../../tensor-product.md), so

$$
\phi_s^*(S\otimes T)=\phi_s^*S\otimes\phi_s^*T.
$$

The ordinary [product rule](../../../../../../product-rule.md) for differentiation therefore yields

$$
\boxed{\mathcal L_X(S\otimes T)=(\mathcal L_XS)\otimes T+S\otimes(\mathcal L_XT).}
$$

This proves the contraction and [Leibniz rule](../../../../../../leibniz-rule.md) properties for all smooth generators, without needing straightening coordinates.

The suggested [flow-box theorem](../../../../../../straightening-theorem.md) applies locally only where $X\ne0$. For example $X=x\partial_x$ vanishes at $x=0$, so it cannot equal a coordinate basis vector there. Its local flow is nevertheless $\phi_s(x)=e^sx$ and $\phi_s^*dx=e^s dx$, giving $\mathcal L_Xdx=dx$ even at that zero. This [Lie derivative at a zero of its generator](../../../../../../lie-derivative-at-a-zero-of-its-generator.md) illustrates why the general flow proof is needed to cover every point.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
