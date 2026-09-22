<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The relevant cycle types are $(5,1)$, $(2,2,2)$ and $(3,2,1)$. Conjugate the first entry to $\alpha=(1\,2\,3\,4\,5)$, fixing six. An entry $\beta$ of type $(2,2,2)$ pairs six with one of the five other letters. Powers of $\alpha$ move that partner to one. With the pair $(1\,6)$ fixed, only three matchings remain:

$$
\begin{array}{c|c}
\beta&\text{cycle type of }\alpha\beta\\
(1\,6)(2\,3)(4\,5)&(4,1,1)\\
(1\,6)(2\,4)(3\,5)&(6)\\
(1\,6)(2\,5)(3\,4)&(3,2,1).
\end{array}
$$

Thus there is exactly one [centralizer](../../../../../../centralizer.md) orbit of eligible second entries, consisting of five matchings before normalization. The third entry is forced to be $(\alpha\beta)^{-1}$, so there is at most one inner orbit of product-one tuples of these types.

For the actual displayed $g_2$, direct multiplication gives

$$
\alpha g_2=(1\,3)(4\,6\,5),\qquad
(\alpha g_2)^{-1}=(1\,3)(4\,5\,6),
$$

which belongs to the class of the displayed $g_3$. This is a product-one witness. The three displayed [permutations](../../../../../../permutation.md) themselves need not multiply to one; the problem concerns their conjugacy classes.

The group $\langle\alpha,g_2\rangle$ is transitive, because $\alpha$ moves the first five points transitively and $g_2$ connects six to them. Its stabilizer of six contains the five-cycle $\alpha$ and is transitive on the other points. Hence the group is [two-transitive](../../../../../../two-transitive-group-action.md) and therefore primitive. Moreover $(\alpha g_2)^3=(1\,3)$ is a [transposition](../../../../../../transposition-permutation.md). The primitive [transposition](../../../../../../transposition-permutation.md) lemma proves that the group is $S_6$. Consequently all tuples in the sole inner orbit generate $S_6$, and

$$
\boxed{(C_{(5,1)},C_{(2,2,2)},C_{(3,2,1)})\text{ is rigid in }S_6.}
$$

As a count check, there are $6\cdot4!=144$ first entries and five eligible second entries for each, giving $720$ tuples. A generating tuple has simultaneous stabilizer equal to the trivial center of $S_6$, so its inner orbit also has size $720$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
