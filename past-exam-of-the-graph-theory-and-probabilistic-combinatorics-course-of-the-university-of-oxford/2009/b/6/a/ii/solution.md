<h1 id="b/6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [asymmetric Lovász local lemma](../../../../../../asymmetric-lovasz-local-lemma.md) states that if there are numbers $0\leq x_i<1$ with

$$
\mathbb P(A_i)\leq x_i\prod_{j\in\Gamma^+(i)}(1-x_j)
$$

for every index, then

$$
\mathbb P\left(\bigcap_i A_i^c\right)\geq\prod_i(1-x_i)>0.
$$

For maximum out-degree $d\geq1$, take every $x_i=1/(d+1)$. Since

$$
\left(1-\frac1{d+1}\right)^d=\left(1+\frac1d\right)^{-d}\geq e^{-1},
$$

one has $x_i(1-x_i)^d\geq1/[e(d+1)]\geq p$. Fewer than $d$ outgoing neighbours only increases the product, so the hypothesis is satisfied whenever $ep(d+1)\leq1$.

If $d=0$, take $x_i=p<1$; the neighbour products are empty and equal one. This separately covers the case in which $1/(d+1)$ would equal the forbidden value one. Thus the **symmetric local lemma** follows in every case.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [B](../../../../b.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../split.md)
7. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
