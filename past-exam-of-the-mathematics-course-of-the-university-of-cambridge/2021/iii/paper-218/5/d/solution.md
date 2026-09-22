<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A weighted nearest-neighbours classifier predicts one when

$$
\sum_{i=1}^kw_iY_{(i)}\geq\frac12,
\qquad w_i\geq0,\quad\sum_iw_i=1,
$$

where neighbours are distance ordered. Under the usual smooth-density and smooth-regression assumptions, asymptotically optimal weights downweight distant neighbours, for example normalized positive parts of $1-(i/k)^{2/p}$. The optimal weighted-nearest-neighbour theorem gives smaller leading asymptotic regret than equal weights.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
