<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**$\boxed{BS(3,4)\text{ is not residually finite}.}$** We exhibit a nonidentity element killed by every finite quotient.

In any finite image, let $r$ be the order of the image of $a$. The relation conjugating $a^3$ to $a^4$ gives

$$
\frac r{\gcd(r,3)}=\frac r{\gcd(r,4)}.
$$

Thus $\gcd(r,3)=\gcd(r,4)=1$. Since $3$ is invertible modulo $r$, the relation implies that the image of $bab^{-1}$ is a power of the image of $a$. Therefore every finite image kills the [group commutator](../../../../../../group-commutator.md)

$$
w=[a,bab^{-1}]=a^{-1}b a^{-1}b^{-1}a b a b^{-1},
$$

using $[s,t]=s^{-1}t^{-1}st$.

View $BS(3,4)$ as an [HNN extension](../../../../../../hnn-extension.md) of $\langle a\rangle\cong\mathbb Z$, with associated subgroups $\langle a^3\rangle$ and $\langle a^4\rangle$. A [pinch in an HNN extension](../../../../../../pinch-in-an-hnn-extension.md) would be $ba^{3j}b^{-1}$ or $b^{-1}a^{4j}b$. The word $w$ has none: its intervening exponents are $-1,1,1$, incompatible with the required divisibilities $3,4,3$. By [Britton's lemma](../../../../../../britton-s-lemma.md), $w\ne1$. Hence finite quotients fail to separate this nonidentity element, proving the conclusion.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
