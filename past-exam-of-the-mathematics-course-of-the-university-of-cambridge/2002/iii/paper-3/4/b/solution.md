<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $n\geq3$, take $C_1$ to be the class of $n$-cycles, $C_2$ the class of [transpositions](../../../../../../transposition-permutation.md), and $C_3$ the class of an $(n-1)$-cycle with one fixed point. With rightmost [permutations](../../../../../../permutation.md) applied first, a witness is

$$
\alpha=(1\,2\,\cdots\,n),\qquad\beta=(1\,2),\qquad
\gamma=(\alpha\beta)^{-1}.
$$

Multiplying an $n$-cycle by a [transposition](../../../../../../transposition-permutation.md) splits it at the two exchanged letters. The resulting cycles have the lengths of the two arcs between those letters in the cyclic ordering. Thus $\alpha\beta$ has type $(n-1,1)$ exactly when the exchanged letters are cyclically adjacent.

Any product-one tuple can first be conjugated so that its first entry is $\alpha$. Its second entry is then one of the $n$ adjacent [transpositions](../../../../../../transposition-permutation.md). The [centralizer](../../../../../../centralizer.md) $\langle\alpha\rangle$ acts transitively on these choices; the third entry is forced to be the inverse product. Therefore every product-one tuple lies in a single simultaneous-conjugation orbit.

The conjugates $\alpha^j\beta\alpha^{-j}$ exchange all adjacent letters around the cycle. Their connected-edge graph generates $S_n$, so the witness, and every tuple in that orbit, generates $S_n$. Hence

$$
\boxed{(C_{(n)},C_{(2,1^{n-2})},C_{(n-1,1)})\text{ is a rigid triple in }S_n.}
$$

For $n=3$ the last two classes coincide, which causes no difficulty: the same three adjacent swaps form one orbit and generate $S_3$.

## ↑ Ancestors (11)

1. [B](../b.md)
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
