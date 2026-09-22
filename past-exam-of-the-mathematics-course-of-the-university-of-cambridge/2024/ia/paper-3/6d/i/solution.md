<h1 id="6d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

From $bab^{-1}=a^{-1}$ we obtain $ba=a^{-1}b$. Moving every occurrence of $b$ to the right and replacing $b^2$ by $a^n$ shows that every [group](../../../../../../group-split.md) element has the form

$$
a^k\quad\hbox{or}\quad a^kb,
\qquad 0\leq k<2n.
$$

The element $b$ cannot lie in $\langle a\rangle$: otherwise it would commute with $a$, forcing $a=a^{-1}$, contrary to $a$ having order $2n>2$. Thus the two cosets $\langle a\rangle$ and $\langle a\rangle b$ are disjoint and each has $2n$ elements. Hence every $n$-dicyclic [group](../../../../../../group-split.md) has order $4n$.

Existence is explicit. Put $\zeta=e^{\pi i/n}$ and take

$$
a=\begin{pmatrix}\zeta&0\\0&\zeta^{-1}\end{pmatrix},
\qquad
b=\begin{pmatrix}0&1\\-1&0\end{pmatrix}.
$$

Then $a$ has order $2n$,

$$
b^2=-I=a^n,
\qquad bab^{-1}=a^{-1}.
$$

The $2n$ diagonal [matrices](../../../../../../matrix.md) $a^k$ and the $2n$ off-diagonal [matrices](../../../../../../matrix.md) $a^kb$ are distinct, so they form a [dicyclic group](../../../../../../dicyclic-group.md) of order $4n$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6D](../../6d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
