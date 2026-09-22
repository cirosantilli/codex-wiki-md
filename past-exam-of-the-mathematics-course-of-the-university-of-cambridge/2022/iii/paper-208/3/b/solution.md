<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Moving one ball can destroy at most one empty bin and create at most one empty bin; the net number of empty bins therefore changes by at most one. Thus $f$ has the [bounded differences property](../../../../../../bounded-differences-property.md) with $c_j=1$ for all $m$ ball coordinates. The upper- and lower-tail forms of the [McDiarmid inequality](../../../../../../mcdiarmid-s-inequality.md) give, for $t>0$,

$$
\boxed{\mathbb P(Z-\mathbb EZ\geq t)
\leq e^{-2t^2/m},
\qquad
\mathbb P(Z-\mathbb EZ\leq-t)
\leq e^{-2t^2/m}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
