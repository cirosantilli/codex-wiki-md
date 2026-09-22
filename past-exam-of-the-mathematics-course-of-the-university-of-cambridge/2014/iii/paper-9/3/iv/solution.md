<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Define $D_{\mathcal G}(A)=\{x:A-x\in\mathcal G\}$. The proposed [addition of filters on the natural numbers](../../../../../../addition-of-filters-on-the-natural-numbers.md) is

$$
\mathcal F+\mathcal G=\{A:D_{\mathcal G}(A)\in\mathcal F\}.
$$

Because addition of positive integers stays in $\mathbb N$, $D_{\mathcal G}(\mathbb N)=\mathbb N$ and $D_{\mathcal G}(\varnothing)=\varnothing$. Thus the sum contains the whole set and excludes the empty set. If $A\subseteq B$, upward closure of $\mathcal G$ gives $D_{\mathcal G}(A)\subseteq D_{\mathcal G}(B)$, so upward closure of $\mathcal F$ gives upward closure of the sum.

Finally, for every $x$,

$$
(A\cap B)-x=(A-x)\cap(B-x).
$$

The conjunction property for $\mathcal G$ proved in (i) consequently gives

$$
D_{\mathcal G}(A\cap B)=D_{\mathcal G}(A)\cap D_{\mathcal G}(B).
$$

Finite-intersection closure of $\mathcal F$ proves the same closure for its sum. All proper-filter axioms hold, so **(iv) is always true**. No ultrafilter assumption is needed here.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
