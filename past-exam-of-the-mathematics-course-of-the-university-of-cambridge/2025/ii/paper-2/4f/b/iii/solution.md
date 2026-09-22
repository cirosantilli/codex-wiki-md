<h1 id="4f/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

This language is not context-free. Intersect it with the regular language

$$
R=0^+1^+0^+.
$$

An even palindrome in $R$ has the form $0^r1^{2s}0^r$, and its first half is $w=0^r1^s$. The required equality of the numbers of zeros and ones in $w$ forces $r=s$. Hence the intersection is

$$
L\cap R=\{0^n1^{2n}0^n:n>0\}.
$$

This is not context-free: applying the pumping lemma to $0^p1^{2p}0^p$, a pumped substring of length at most $p$ cannot meet both zero blocks. Pumping therefore either destroys equality of the two zero counts or changes the middle count away from twice their common value.

Context-free languages are closed under intersection with regular languages, so a context-free $L$ would make $L\cap R$ context-free. This contradiction proves the claim.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4F](../../../4f.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
