<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Precomposition defines

$$
f^*:[\mathbb D^{\rm op},\mathbf{Set}]\longrightarrow[\mathbb C^{\rm op},\mathbf{Set}],\qquad
P\longmapsto P\circ T^{\rm op}.
$$

It preserves [finite limits](../../../../../../finite-limit.md) because presheaf limits are pointwise. Its [right adjoint](../../../../../../adjoint-functors.md) is a [Right Kan extension](../../../../../../right-kan-extension.md); explicitly, for $H\in\widehat{\mathbb C}$,

$$
(f_*H)(d)=\operatorname{Nat}_{\widehat{\mathbb C}}(\mathbb D(T-,d),H).
$$

Precomposition in $d$ supplies the restriction maps. To verify the [adjunction](../../../../../../adjoint-functors.md), a map $P\circ T^{\rm op}\to H$ sends $x\in P(d)$ to the natural family taking $h:Tc\to d$ to the image in $H(c)$ of $P(h)x$. Conversely evaluate such a family at $d=Tc$, $h=1_{Tc}$; naturality makes the two constructions inverse. Thus $f^*\dashv f_*$ and $f^*$ is left exact, giving the required [geometric morphism](../../../../../../geometric-morphism.md)

$$
\boxed{\widehat{\mathbb C}\longrightarrow\widehat{\mathbb D}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
