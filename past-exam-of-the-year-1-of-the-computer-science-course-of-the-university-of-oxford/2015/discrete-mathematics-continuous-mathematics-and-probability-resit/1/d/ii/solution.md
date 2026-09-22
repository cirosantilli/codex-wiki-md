<h1 id="1/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First suppose the [sets](../../../../../../set-split.md) are finite, with [cardinalities](../../../../../../cardinality.md) $a=|A|\geq2$ and $b=|B|\geq2$. The [power set](../../../../../../power-set.md) and [Cartesian product](../../../../../../cartesian-product.md) counting rules give

$$
|\mathcal P(A\times B)|=2^{ab},\qquad
|\mathcal P(A)\times\mathcal P(B)|=2^{a+b}.
$$

Since $ab-a-b=(a-1)(b-1)-1\geq0$, the desired inequality follows.

The [power-set product cardinality inequality](../../../../../../power-set-product-cardinality-inequality.md) also has an [injection](../../../../../../injective-function.md) proof that does not assume finiteness. Choose distinct $a_0,a_1\in A$ and distinct $b_0,b_1\in B$. For $S\subseteq A$ and $T\subseteq B$, define the [subset](../../../../../../subset.md) of $A\times B$

$$
\Phi(S,T)=(S\times\{b_0\})\cup(\{a_0\}\times(T\setminus\{b_0\}))\cup E_T,
\qquad
E_T=\begin{cases}\{(a_1,b_1)\},&b_0\in T,\\\varnothing,&b_0\notin T.\end{cases}
$$

These three encoding regions are disjoint. The row with second coordinate $b_0$ recovers $S$; the column with first coordinate $a_0$ and second coordinate different from $b_0$ recovers $T\setminus\{b_0\}$; the extra position $(a_1,b_1)$ records whether $b_0\in T$. Thus $\Phi$ is [injective](../../../../../../injective-function.md), proving for arbitrary [sets](../../../../../../set-split.md)

$$
\boxed{|\mathcal P(A\times B)|\geq|\mathcal P(A)\times\mathcal P(B)|.}
$$

Encoding by $S\times T$ alone would fail: all pairs with either factor empty would have the same output.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
