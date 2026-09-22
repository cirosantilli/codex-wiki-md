<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply the same [pumping of a group multiplier automaton](../../../../../../../pumping-of-a-group-multiplier-automaton.md) to the accepted pair containing the given representative $u$. Since $|u|>|w|+N$, there is a nonempty loop entirely after the tape containing $w$ has ended. Write $u=pqr$, with $q\ne\varepsilon$ the letters read during this loop. Repeating the loop any number of times leaves the other tape equal to $w$, and the [group multiplier automaton](../../../../../../../group-multiplier-automaton.md) accepts the resulting [padded convolution of words](../../../../../../../padded-convolution-of-words.md). Consequently

$$
\boxed{pq^kr\in L,\qquad \overline{pq^kr}=g\quad(k\geq0).}
$$

These [words over an alphabet](../../../../../../../string.md) have distinct lengths because $|q|>0$. Hence **there are infinitely many representatives of $g$ in $L$**. No uniqueness of representatives was assumed in either part.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 120](../../../../paper-120-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
