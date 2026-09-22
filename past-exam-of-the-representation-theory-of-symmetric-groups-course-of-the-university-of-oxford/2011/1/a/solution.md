<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Murnaghan–Nakayama rule](../../../../murnaghan-nakayama-rule.md) computes an [irreducible character](../../../../irreducible-character.md) on a [permutation](../../../../permutation.md) with a specified cycle of [length](../../../../length.md) $r$ by

$$
\boxed{\chi_\lambda((r)\rho)=\sum_{\substack{\nu\vdash n-r\\\lambda/\nu\text{ a rim hook of size }r}}(-1)^{\ell(\lambda/\nu)}\chi_\nu(\rho).}
$$

Here the leg [length](../../../../length.md) is one less than the number of occupied rows, and iteration ends at the empty [partition](../../../../partition-of-an-integer.md) with [character](../../../../character-of-a-representation.md) value one. Conjugating a [partition](../../../../partition-of-an-integer.md) twists its [character](../../../../character-of-a-representation.md) by the sign [character](../../../../character-of-a-representation.md):

$$
\boxed{\chi_{\lambda'}(\sigma)=\operatorname{sgn}(\sigma)\chi_\lambda(\sigma).}
$$

For a [transposition](../../../../transposition-permutation.md), remove a rim domino and evaluate the remaining [character](../../../../character-of-a-representation.md) at the identity of $S_3$. The three possible remaining shapes $(3),(2,1),(1^3)$ have degrees $1,2,1$ by the [hook](../../../../hook-of-a-young-diagram.md) formula. For $(5)$ the single removable horizontal domino leaves $(3)$, giving one. For $(4,1)$ the only rim domino leaves $(2,1)$, giving two. For $(3,2)$ the removable bottom-row domino leaves $(3)$, giving one. For $(3,1,1)$, a horizontal domino leaves $(1^3)$ and a vertical domino leaves $(3)$; their contributions are $1-1=0$. The conjugate-partition identity gives the remaining three values with reversed sign.

The [Hook-length formula](../../../../hook-length-formula.md) is $\chi_\lambda(1)=5!/\prod_{u\in[\lambda]}h(u)$. Both requested columns are therefore

$$
\boxed{\begin{array}{c|r|r|r}
\lambda&\prod h(u)&\chi_\lambda(1)&\chi_\lambda((12))\\\hline
(5)&120&1&1\\
(4,1)&30&4&2\\
(3,2)&24&5&1\\
(3,1,1)&20&6&0\\
(2,2,1)&24&5&-1\\
(2,1,1,1)&30&4&-2\\
(1^5)&120&1&-1
\end{array}}
$$

As a check, the squared degrees sum to $1+16+25+36+25+16+1=120=|S_5|$. The [transposition](../../../../transposition-permutation.md) column above was obtained from rim-hook removal and conjugation, independently of [permutation characters](../../../../permutation-character.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the representation Theory of Symmetric Groups course of the University of Oxford](../../../split.md)
5. [Representation Theory of Symmetric Groups course of the University of Oxford](../../../../representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
