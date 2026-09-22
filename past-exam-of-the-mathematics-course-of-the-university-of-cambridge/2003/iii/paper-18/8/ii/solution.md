<h1 id="8/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $F\dashv G$ with unit $\eta$ and counit $\varepsilon$, set

$$
\boxed{T=GF,\qquad\mu_A=G\varepsilon_{FA},\qquad\text{unit }\eta_A.}
$$

Naturality of the unit and counit makes these [natural transformations](../../../../../../natural-transformation.md). The two triangle identities give $\mu_A\eta_{TA}=1_{TA}$ and $\mu_AT\eta_A=1_{TA}$. Naturality of $\varepsilon$ at $\varepsilon_{FA}$ gives $\varepsilon_{FA}\varepsilon_{FGFA}=\varepsilon_{FA}FG\varepsilon_{FA}$. Applying $G$ proves $\mu_A\mu_{TA}=\mu_AT\mu_A$. Thus this is the [monad induced by an adjunction](../../../../../../monad-induced-by-an-adjunction.md).

Conversely, for any [monad](../../../../../../monad.md) take the free-algebra [functor](../../../../../../functor.md) $F^T(A)=(TA,\mu_A)$ and the forgetful [functor](../../../../../../functor.md) $U:\mathcal C^T\to\mathcal C$. For an algebra $(B,b)$, the assignments $h\mapsto h\eta_A$ and $k\mapsto bT(k)$ give inverse bijections between algebra maps $F^T(A)\to(B,b)$ and arrows $A\to B$. For the inverse identities, $bT(k)\eta_A=b\eta_Bk=k$, while $bT(h\eta_A)=h\mu_AT\eta_A=h$. The algebra and [monad](../../../../../../monad.md) laws also make $bT(k)$ an algebra morphism, since $bT(k)\mu_A=b\mu_BT^2k=bT(b)T^2k$. These bijections are natural, giving the [free-forgetful Eilenberg-Moore adjunction](../../../../../../free-forgetful-eilenberg-moore-adjunction.md). Its unit is $\eta$, its counit at $(B,b)$ is $b$, and its induced multiplication is exactly $\mu$. Thus **every [monad](../../../../../../monad.md) arises from an [adjunction](../../../../../../adjoint-functors.md)**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [8](../../8.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
