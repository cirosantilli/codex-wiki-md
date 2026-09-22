<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $A$ is empty, take the zero [generalized character](../../../../../../virtual-character.md); if $B$ is empty, take the [trivial character](../../../../../../trivial-character.md). Otherwise let $\pi$ be the set of primes dividing the orders of elements of $A$. The coprimality hypothesis makes every element of $B$ a $\pi'$-element. Thus every nonidentity element of $G$ is either a [pi-element](../../../../../../pi-element.md) in $A$ or a complementary-prime element in $B$. In particular these sets are unions of [conjugacy classes](../../../../../../conjugacy-class.md), since conjugation preserves element order.

Put $m=|G|_\pi$ and $n=|G|_{\pi'}$. Their [greatest common divisor](../../../../../../greatest-common-divisor.md) is one, so the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) supplies an integer $d$ such that

$$
d\equiv1\pmod m,\qquad d\equiv0\pmod n.
$$

Define the [class function](../../../../../../class-function.md) $f$ by $f(1)=d$, $f=1$ on $A$ and $f=0$ on $B$. We verify [Brauer's characterization of characters](../../../../../../brauer-s-characterization-of-characters.md) directly.

For an [elementary subgroup](../../../../../../elementary-group.md) $E=P\times C$, the cyclic factor can be split into its $\pi$-part and $\pi'$-part. Attach $P$ to the part containing its prime. This expresses $E=E_\pi\times E_{\pi'}$. Both factors cannot be nontrivial: choosing a nonidentity element in each would give a commuting product of mixed prime order, whereas every element of $G$ has order involving only one of the two prime sets. Hence $E$ is wholly a $\pi$-group or wholly a $\pi'$-group.

Let $r_E$ be the [character](../../../../../../character-of-a-representation.md) of the [regular representation](../../../../../../regular-representation.md) of $E$, with value $|E|$ at the identity and zero elsewhere. In the two cases respectively,

$$
f_E=1_E+\frac{d-1}{|E|}r_E,\qquad
f_E=\frac d{|E|}r_E.
$$

The coefficients are integers because $|E|$ divides $m$ or $n$. Thus both are [generalized characters](../../../../../../virtual-character.md). The trivial [subgroup](../../../../../../subgroup.md) causes no difficulty since $d$ is an integer. By [Brauer's characterization of characters](../../../../../../brauer-s-characterization-of-characters.md), $f$ is a [generalized character](../../../../../../virtual-character.md) of $G$.

**Taking $\vartheta=f$ gives the required values.**

This is a [generalized character separating complementary prime elements](../../../../../../generalized-character-separating-complementary-prime-elements.md); the freely chosen value at the identity is what makes all elementary restrictions integral.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
