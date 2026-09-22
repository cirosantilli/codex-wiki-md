<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [Elston-Stewart algorithm](../../../../../../elston-stewart-algorithm.md) first sums over the child:

$$
L=\sum_{g=0}^1a_gp_g\left(b_0t_{0\mid g}+b_1t_{1\mid g}\right).
$$

For each of the two parent states, the inner message requires two multiplications and one addition, totaling four multiplications and two additions. Multiplying each message by its two parent factors takes two further multiplications per parent state, totaling four. The final sum uses one addition. Therefore

$$
\boxed{8\text{ multiplications},\qquad3\text{ additions}.}
$$

Moving the sum inward saves four multiplications because the factors independent of the child [genotype](../../../../../../genotype.md) are evaluated only once per parent state.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
