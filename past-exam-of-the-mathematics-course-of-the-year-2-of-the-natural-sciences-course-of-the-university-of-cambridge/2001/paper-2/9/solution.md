<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

**Definitions.** A [group homomorphism](../../../../group-homomorphism.md) $\varphi:G_1\to G_2$ preserves multiplication, $\varphi(xy)=\varphi(x)\varphi(y)$. A [group isomorphism](../../../../group-isomorphism.md) is a bijective [group homomorphism](../../../../group-homomorphism.md). The [kernel of a group homomorphism](../../../../kernel-of-a-group-homomorphism.md) is

$$
\boxed{K=\ker\varphi=\{x\in G_1:\varphi(x)=e_2\}.}
$$

Preserving multiplication implies $\varphi(e_1)=e_2$ and $\varphi(x^{-1})=\varphi(x)^{-1}$: the first follows by cancelling $\varphi(e_1)$ from its square, and the second follows by applying $\varphi$ to $xx^{-1}=e_1$.

**Kernel subgroup.** The identity belongs to $K$. For $x,y\in K$, $\varphi(xy)=e_2e_2=e_2$, so $xy\in K$. Also $\varphi(x^{-1})=e_2^{-1}=e_2$, so $x^{-1}\in K$. Thus $\boxed{K\leq G_1}$.

**Normality.** For $g\in G_1$ and $k\in K$,

$$
\varphi(gkg^{-1})=\varphi(g)\varphi(k)\varphi(g)^{-1}=\varphi(g)e_2\varphi(g)^{-1}=e_2.
$$

Hence every $gkg^{-1}$ is again in $K$, proving $\boxed{K\trianglelefteq G_1}$. Applying the same statement with $g^{-1}$ gives equality $gKg^{-1}=K$, and therefore $gK=Kg$.

**Group of cosets.** Define the product on the [left cosets](../../../../left-coset.md) by

$$
\boxed{(aK)(bK)=(ab)K.}
$$

To check that this does not depend on representatives, replace $a,b$ by $ak_1,bk_2$. Then

$$
(ak_1)(bk_2)=ab(b^{-1}k_1b)k_2\in abK,
$$

because normality puts $b^{-1}k_1b$ in $K$. Thus the product is well defined. It is associative because multiplication in $G_1$ is associative; its identity is $K=e_1K$, and the inverse of $aK$ is $a^{-1}K$. Consequently the cosets form the [quotient group](../../../../quotient-group.md) $\boxed{G_1/K}$.

The map $aK\mapsto\varphi(a)$ is well defined and gives an isomorphism $G_1/K\cong\operatorname{im}\varphi$. If the original mapping is onto $G_2$, this becomes $G_1/K\cong G_2$. No surjectivity is needed for the [kernel of a group homomorphism](../../../../kernel-of-a-group-homomorphism.md) to be a [normal subgroup](../../../../normal-subgroup.md) or for the [quotient group](../../../../quotient-group.md) to exist.

## ↑ Ancestors (12)

1. [9](../9.md)
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
