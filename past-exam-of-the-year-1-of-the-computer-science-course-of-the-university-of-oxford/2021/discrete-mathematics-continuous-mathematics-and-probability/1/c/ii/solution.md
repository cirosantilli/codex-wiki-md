<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $d=\gcd(c,n)$, $c=dc'$, and $n=dn'$. The preceding part gives $\gcd(c',n')=1$. The [integer congruence](../../../../../../integer-congruence.md) on the left is equivalent to

$$
n\mid c(a-b)
\quad\Longleftrightarrow\quad
n'\mid c'(a-b).
$$

By [Euclid's lemma](../../../../../../euclid-s-lemma.md), coprimality of $c'$ and $n'$ makes this equivalent to $n'\mid a-b$. The reverse implication is also immediate by multiplying a [divisibility](../../../../../../divisibility-split.md) relation by $dc'$. Therefore

$$
\boxed{ac\equiv bc\pmod n
\quad\Longleftrightarrow\quad
 a\equiv b\pmod{n/\gcd(c,n)}.}
$$

This is [cancellation of a common factor in a congruence](../../../../../../cancellation-of-a-common-factor-in-a-congruence.md). The printed equality sign in the right-hand expression is interpreted as equality of [residue classes](../../../../../../residue-class.md), hence the displayed [integer congruence](../../../../../../integer-congruence.md). Ordinary equality of the [integers](../../../../../../integer-split.md) $a,b$ would be false: the following example has $a\ne b$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
