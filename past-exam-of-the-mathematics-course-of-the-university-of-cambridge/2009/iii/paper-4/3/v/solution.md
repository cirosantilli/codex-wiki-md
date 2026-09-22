<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Take $g=(1\ 2\ \cdots\ n)$. Since $n\equiv3\pmod4$ is odd, its sign is $(-1)^{n-1}=1$, so $g\in A_n$. Define $s$ to fix $1$ and reverse the other cyclic labels: it interchanges $2$ with $n$, $3$ with $n-1$, and so on. Then $sgs^{-1}=g^{-1}$, while

$$
\operatorname{sgn}(s)=(-1)^{(n-1)/2}=-1.
$$

The [centralizer](../../../../../../centralizer.md) of an $n$-cycle in $S_n$ is $\langle g\rangle$: a commuting permutation is determined by the image of one point, and that image fixes the corresponding power of the cycle. All its elements are even, because $g$ is even. Any other conjugator taking $g$ to $g^{-1}$ differs from $s$ by a [centralizer](../../../../../../centralizer.md) element and therefore remains odd. Thus $g$ and $g^{-1}$ are not conjugate in $A_n$. This is the parity obstruction described by [inversion of an odd cycle in an alternating group](../../../../../../inversion-of-an-odd-cycle-in-an-alternating-group.md).

For any complex character of a finite group, a unitary realization gives

$$
\theta(g^{-1})=\overline{\theta(g)}.
$$

If every $\theta\in\operatorname{Irr}(A_n)$ had real value at $g$, all these characters would take equal values on $g$ and $g^{-1}$. But [irreducible characters separate conjugacy classes](../../../../../../irreducible-characters-separate-conjugacy-classes.md): they form a basis of [class functions](../../../../../../class-function.md), so equality of every irreducible value would also give equality of the class indicator functions. The two distinct [conjugacy classes](../../../../../../conjugacy-class.md) cannot have that property. Consequently

$$
\boxed{\text{There is }\theta\in\operatorname{Irr}(A_n)\text{ with }\theta((1\ 2\ \cdots\ n))\notin\mathbb R.}
$$

In other words, these alternating groups are not [ambivalent groups](../../../../../../ambivalent-group.md), even though all symmetric-group [irreducible characters](../../../../../../irreducible-character.md) are integer-valued.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [3](../../3.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
