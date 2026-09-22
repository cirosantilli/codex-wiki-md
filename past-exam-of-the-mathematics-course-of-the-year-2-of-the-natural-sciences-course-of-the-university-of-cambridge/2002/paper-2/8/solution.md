<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

**Cosets and counting.** A [left coset](../../../../left-coset.md) of a [subgroup](../../../../subgroup.md) $H$ in a [group](../../../../group-split.md) $G$ is $gH=\{gh:h\in H\}$. The [left cosets](../../../../left-coset.md) partition $G$ and each has $|H|$ elements. [Lagrange's theorem](../../../../lagrange-s-theorem.md) states that for a finite [group](../../../../group-split.md), $\boxed{|G|=[G:H]|H|}$; in particular, the [subgroup](../../../../subgroup.md) order divides the [group order](../../../../order-of-a-finite-group.md).

**The matrix group.** Work throughout in the [finite field](../../../../finite-field.md) $\mathbb F_5$, so every nonzero entry has a multiplicative inverse. Denote a matrix by $A(a,b,c)$, with $a,c\ne0$. Ordinary [matrix multiplication](../../../../matrix-multiplication.md), interpreted using [modular arithmetic](../../../../modular-arithmetic-split.md), gives

$$
A(a,b,c)A(d,e,f)=A(ad,ae+bf,cf).
$$

Its diagonal entries remain nonzero, proving closure. Associativity is inherited from [matrix multiplication](../../../../matrix-multiplication.md), $A(1,0,1)$ is the [identity element](../../../../identity-element.md), and

$$
\boxed{A(a,b,c)^{-1}=A(a^{-1},-a^{-1}bc^{-1},c^{-1}).}
$$

This lies in the same set and multiplication checks the inverse in either order. Thus these matrices form a [group](../../../../group-split.md). There are four choices each for $a$ and $c$ and five for $b$, giving $\boxed{|G|=4\cdot5\cdot4=80}$.

**The subgroup.** Write $h(a,c)=A(a,a-c,c)$. Then

$$
h(a,c)h(d,f)=A(ad,a(d-f)+(a-c)f,cf)=h(ad,cf).
$$

It contains the identity $h(1,1)$, is closed, and has inverse $h(a^{-1},c^{-1})$. Interchanging the two factors leaves the product unchanged because multiplication in $\mathbb F_5$ is commutative. Therefore $H$ is an [abelian subgroup](../../../../abelian-subgroup.md), with

$$
\boxed{|H|=4^2=16,\qquad [G:H]=80/16=5.}
$$

Equivalently $H$ is isomorphic to $\mathbb F_5^\times\times\mathbb F_5^\times$ by $h(a,c)\mapsto(a,c)$, which also explains its abelian property. Its order divides $80$, verifying [Lagrange's theorem](../../../../lagrange-s-theorem.md).

There are five distinct [left cosets](../../../../left-coset.md). Representatives can be taken as $U_t=A(1,t,1)$, $t\in\mathbb F_5$: indeed

$$
U_th(a,c)=A(a,a-c+tc,c),\qquad t=(b-a+c)c^{-1}.
$$

Every matrix lies in exactly the coset specified by this unique $t$.

**Elements whose square is the identity.** Squaring gives

$$
A(a,b,c)^2=A(a^2,b(a+c),c^2).
$$

Thus $a,c\in\{1,-1\}=\{1,4\}$ and $b(a+c)=0$. For equal signs, $a+c\ne0$ in $\mathbb F_5$, so $b=0$. For opposite signs, $a+c=0$ and all five $b$ values work. The complete set is therefore

$$
\boxed{\{I,-I\}\ \cup\ \left\{\begin{pmatrix}1&b\\0&-1\end{pmatrix}:b\in\mathbb F_5\right\}\ \cup\ \left\{\begin{pmatrix}-1&b\\0&1\end{pmatrix}:b\in\mathbb F_5\right\}.}
$$

It contains $2+5+5=12$ elements, including the identity; the other eleven are [involutions](../../../../involution.md). Since $12$ does not divide $80$, [Lagrange's theorem](../../../../lagrange-s-theorem.md) proves that this set is not a [subgroup](../../../../subgroup.md).

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 2](../../paper-2-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
