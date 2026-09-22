<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The base [free product](../../../../../../free-product.md) for the [group encoding of a modular machine](../../../../../../group-encoding-of-a-modular-machine.md) is

$$
\boxed{K=\langle x,y,t\mid xy=yx\rangle\cong\mathbb Z^2*\mathbb Z,\qquad
 t(r,s)=x^{-r}y^{-s}t x^r y^s.}
$$

The letters $x,y$ generate the first factor, and $t$ generates the second. Let $T_K$ be the [kernel](../../../../../../kernel-of-a-linear-map.md) of the [group homomorphism](../../../../../../group-homomorphism.md) $K\to\langle x,y\rangle\cong\mathbb Z^2$ that kills $t$. Then

$$
T_K=\langle t(r,s):r,s\in\mathbb Z\rangle
$$

is a [free group](../../../../../../free-group.md) with this displayed [free basis of a group](../../../../../../free-basis-of-a-group.md). Indeed every word in $K$ can be rewritten as a product of such conjugates followed by an element of $\langle x,y\rangle$, so they generate the kernel. A freely reduced product of these conjugates is nontrivial by the [normal form theorem for a free product](../../../../../../normal-form-theorem-for-a-free-product.md): after combining adjacent occurrences of the same conjugate, different successive indices give a nonzero intervening $x,y$-syllable. Thus there is no relation among the proposed basis elements.

For clarity, a [modular machine](../../../../../../modular-machine.md) of modulus $m>1$ has at most one instruction for each residue pair $(a,b)$, with $0\le a,b<m$ and $0\le c<m^2$. Its right and left transitions are respectively

$$
(mu+a,mv+b)\longmapsto(m^2u+c,v),\qquad
(mu+a,mv+b)\longmapsto(u,m^2v+c).
$$

Its [halting set at a designated terminal configuration](../../../../../../halting-set-at-a-designated-terminal-configuration.md) $H_0(\mathcal M)$ consists of the nonnegative pairs whose forward computation reaches $(0,0)$, including $(0,0)$ itself. These formulas explain the exponents in the associated-subgroup maps below.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 104](../../../paper-104-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
