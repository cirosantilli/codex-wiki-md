<h1 id="18h/solution">Solution</h1>

↑ **Parent:** [18H](../18h.md)

A useful closed-cover version of the [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) is the following. Let $X=A\cup B$ with $A,B,A\cap B$ path-connected closed subspaces and basepoint in their intersection. Assume there are open neighbourhoods $U,V$ covering $X$ that deformation retract onto $A,B$, while $U\cap V$ deformation retracts onto $A\cap B$, with the induced inclusions compatible up to based homotopy. Then

$$
\pi_1(X)=\pi_1(A)*\pi_1(B)/\langle\!\langle i_A(\gamma)i_B(\gamma)^{-1}:\gamma\in\pi_1(A\cap B)\rangle\!\rangle.
$$

The neighbourhood hypothesis, available for the present finite subcomplex gluing, matters: arbitrary closed covers need not satisfy this theorem.

A [Möbius band](../../../../../mobius-band.md) retracts onto its core circle, with generator $m$; its boundary represents $m^2$. The [torus](../../../../../torus.md) has generators $u,v$ and relation $[u,v]=1$. The attaching circle is the $u$ circle. Reversing the attaching homeomorphism merely replaces $u$ by its inverse and changes no isomorphism type. The closed-cover theorem gives

$$
\boxed{\pi_1(X)=\langle m,u,v\mid [u,v]=1,\ u=m^2\rangle
=\langle m,v\mid[m^2,v]=1\rangle}.
$$

Mapping $m\mapsto0$, $v\mapsto1$ surjects onto $\mathbb Z$, so the group is infinite. Imposing the extra relation $m^2=1$ gives the quotient $C_2*\mathbb Z$, a nonabelian [free product](../../../../../free-product.md), since alternating reduced words $mv$ and $vm$ differ. A quotient of an abelian group would be abelian, so **the [fundamental group](../../../../../fundamental-group.md) is nonabelian**.

## ↑ Ancestors (10)

1. [18H](../18h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
