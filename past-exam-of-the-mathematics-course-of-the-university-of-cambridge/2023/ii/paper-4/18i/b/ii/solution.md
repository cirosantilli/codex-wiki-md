<h1 id="18i/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $x_1,x_2,x_3\in L$ be the distinct roots of $f$, and define the two cyclic sums

$$
r=x_1^2x_2+x_2^2x_3+x_3^2x_1,
\qquad
s=x_2^2x_1+x_3^2x_2+x_1^2x_3.
$$

Vieta's relations in characteristic two are

$$
x_1+x_2+x_3=0,
\qquad
x_1x_2+x_2x_3+x_3x_1=a,
\qquad
x_1x_2x_3=b.
$$

A direct symmetric expansion using these identities gives

$$
r+s=b,
\qquad
rs=a^3+b^2.
$$

Consequently $r$ and $s$ are the roots of the [characteristic-two cubic resolvent](../../../../../../../characteristic-two-cubic-resolvent.md)

$$
g(T)=T^2+bT+a^3+b^2.
$$

They are distinct because $r+s=b\ne0$. Thus $g$ splits into distinct linear factors in $L[T]$.

A three-cycle of the roots fixes each cyclic sum, whereas any transposition interchanges $r$ and $s$. The induced action on $\{r,s\}$ is therefore exactly the sign action of the [symmetric group](../../../../../../../symmetric-group.md) $S_3$ on $S_3/A_3$. If the Galois group $G$ is contained in $A_3$, it fixes $r$ and $s$, so both lie in the fixed field $K$ and $g$ splits over $K$. Conversely, if $g$ splits in $K[T]$, its distinct roots $r,s$ belong to $K$ and every element of $G$ fixes them individually. No element of $G$ can then act as an odd root permutation, so $G\subseteq A_3$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [18I](../../../18i.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
