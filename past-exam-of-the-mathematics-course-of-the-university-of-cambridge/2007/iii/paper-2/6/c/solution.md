<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Read the supplied [tangle](../../../../../../tangle.md) from top to bottom. Its input word is $\downarrow\uparrow\downarrow$, and its output word is $\downarrow$. There are three successive events: the upper crossing of the rightmost two strands, the lower crossing of the leftmost two strands, and the right-hand oriented evaluation. At both crossings, the upper-left-to-lower-right strand passes over; both are therefore $X_+$ in the geometric convention of part (a). The evaluation joins a downward strand to an upward strand, so it is $\overleftarrow{\cup}$.

The elementary factorization is consequently

$$
\boxed{T=(\downarrow\otimes\overleftarrow{\cup})
\circ(X_+\otimes\uparrow)
\circ(\downarrow\otimes X_+).}
$$

Its boundary words give an explicit composition check:

$$
\downarrow\uparrow\downarrow
\longrightarrow\downarrow\downarrow\uparrow
\longrightarrow\downarrow\downarrow\uparrow
\longrightarrow\downarrow.
$$

The third panel in part (b) draws these slices. Sliding the right-hand evaluation downwards and straightening the identity portions gives the PDF diagram without changing either crossing's overpass. If the names $X_+,X_-$ are interchanged in another crossing convention, both displayed crossings must be renamed together; the stated overpasses determine the actual [tangle](../../../../../../tangle.md) independently of those names.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
