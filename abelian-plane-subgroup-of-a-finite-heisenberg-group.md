# Abelian plane subgroup of a finite Heisenberg group

↑ **Parent:** [Heisenberg group over a prime field](heisenberg-group-over-a-prime-field.md)

Use the coordinate convention

$$
A(a,b,c)=\begin{pmatrix}1&a&b\\0&1&c\\0&0&1\end{pmatrix},\qquad a,b,c\in\mathbb F_p.
$$

In this convention the [Heisenberg group over a prime field](heisenberg-group-over-a-prime-field.md) has the product

$$
A(a,b,c)A(a',b',c')=A(a+a',b+b'+ac',c+c').
$$

The subset $H=\{A(t,b,t):t,b\in\mathbb F_p\}$ is an [Abelian subgroup](abelian-subgroup.md) of order $p^2$: the middle coordinate in a product is $b+b'+tt'$, which is symmetric in the factors. Also $A(t,b,t)^{-1}=A(-t,t^2-b,-t)$ lies in $H$. The map $A(a,b,c)\mapsto a-c$ is a surjective [group homomorphism](group-homomorphism.md) to the additive group of $\mathbb F_p$, with [kernel of a group homomorphism](kernel-of-a-group-homomorphism.md) $H$. Hence $H$ is a [normal subgroup](normal-subgroup.md) of [subgroup index](index-of-a-subgroup.md) $p$, and its left [cosets](coset.md) are exactly the level sets of $a-c$.

For odd $p$, an explicit [group isomorphism](group-isomorphism.md) from $H$ to the additive group $\mathbb F_p^2$ is

$$
A(t,b,t)\longmapsto(t,b-t^2/2).
$$

The term $tt'$ in matrix multiplication cancels the cross term in $(t+t')^2/2$. Thus $H$ is an [elementary abelian group](elementary-abelian-group.md), isomorphic to $C_p\times C_p$.

## ↑ Ancestors (7)

1. [Heisenberg group over a prime field](heisenberg-group-over-a-prime-field.md)
2. [Finite group theory](finite-group-theory-split.md)
3. [Group theory](group-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2/9/b/solution.md)
