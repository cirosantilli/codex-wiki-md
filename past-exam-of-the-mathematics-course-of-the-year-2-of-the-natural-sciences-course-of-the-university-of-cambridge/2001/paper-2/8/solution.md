<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

**Cosets and Lagrange.** A [left coset](../../../../left-coset.md) is $gH=\{gh:h\in H\}$. The [left cosets](../../../../left-coset.md) of a [subgroup](../../../../subgroup.md) partition a [group](../../../../group-split.md), each with $|H|$ elements. [Lagrange's theorem](../../../../lagrange-s-theorem.md) states $\boxed{|G|=[G:H]|H|}$ for a finite [group](../../../../group-split.md), so every [subgroup](../../../../subgroup.md) order divides the [group order](../../../../order-of-a-finite-group.md).

**The 64-element group.** Work in the [commutative ring](../../../../commutative-ring.md) $R=\mathbb Z/4\mathbb Z$, which has [zero divisors](../../../../zero-divisor.md). Denote the displayed lower triangular matrix by $A(a,b,c)$, where $a,b,c$ are its three entries below the diagonal. Direct [matrix multiplication](../../../../matrix-multiplication.md) gives

$$
\boxed{A(a,b,c)A(d,e,f)=A(a+d,b+e+cd,c+f).}
$$

All arithmetic is modulo four, so the set is closed. Associativity comes from [matrix multiplication](../../../../matrix-multiplication.md), the [identity element](../../../../identity-element.md) is $A(0,0,0)$, and

$$
\boxed{A(a,b,c)^{-1}=A(-a,ca-b,-c).}
$$

The formula works in either multiplication order and requires no division. Hence these matrices form a [group](../../../../group-split.md) of order $\boxed{|G|=4^3=64}$. This is the lower triangular version of the [Heisenberg group over a commutative ring](../../../../heisenberg-group-over-a-commutative-ring.md).

**The abelian subgroup.** If $a=c$, write $h(a,b)=A(a,b,a)$. Then

$$
h(a,b)h(d,e)=h(a+d,b+e+ad)=h(d,e)h(a,b).
$$

The identity is $h(0,0)$ and the inverse is $h(-a,a^2-b)$, proving an [abelian subgroup](../../../../abelian-subgroup.md). Its two independent entries give $\boxed{|H|=16}$ and $\boxed{[G:H]=4}$, in accordance with [Lagrange's theorem](../../../../lagrange-s-theorem.md). This is the [abelian plane subgroup of the Heisenberg group modulo four](../../../../abelian-plane-subgroup-of-the-heisenberg-group-modulo-four.md).

More explicitly, $A(a,b,c)\mapsto a-c$ is a [surjective group homomorphism](../../../../surjective-group-homomorphism.md) to the additive group of $R$, with kernel $H$. The four [left cosets](../../../../left-coset.md) are exactly the four sets with fixed $a-c=t$, $t=0,1,2,3$; representatives are $A(t,0,0)$. Thus $H$ is also a [normal subgroup](../../../../normal-subgroup.md).

**Matrices squaring to the identity.** The product formula gives

$$
A(a,b,c)^2=A(2a,2b+ca,2c).
$$

The first and third coordinates vanish only when $a,c\in\{0,2\}$. Then $ca=0$ modulo four, so the middle coordinate vanishes exactly when $b\in\{0,2\}$. Therefore the complete set is

$$
\boxed{K=\{A(a,b,c):a,b,c\in\{0,2\}\},\qquad |K|=8.}
$$

It is a [subgroup](../../../../subgroup.md): multiplying two such elements keeps all three entries even, and their cross term $cd$ vanishes modulo four, so the product simply adds the three even coordinates. The identity is included and each element is its own inverse. In fact $K$ is isomorphic to the [direct product of groups](../../../../direct-product-of-groups.md) $C_2\times C_2\times C_2$. The seven nonidentity elements are [involutions](../../../../involution.md).

Finally, the last subset in the PDF is defined by $a\ne0\ne b$, with no restriction on $c$. It has $3\cdot3\cdot4=36$ elements, which cannot be a [subgroup](../../../../subgroup.md) because $36$ does not divide $64$. It also excludes the [identity element](../../../../identity-element.md). Thus

$$
\boxed{\{A(a,b,c):a\ne0,\ b\ne0\}\text{ is not a subgroup}.}
$$

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 2](../../paper-2-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
