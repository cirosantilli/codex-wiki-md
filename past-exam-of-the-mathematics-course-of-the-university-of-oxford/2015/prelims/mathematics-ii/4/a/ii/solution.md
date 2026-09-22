<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose the [continuous function](../../../../../../../continuous-function.md) $f$ did not have [uniform continuity](../../../../../../../uniform-continuity.md) on $[a,b]$. Negating its definition gives $\varepsilon_0>0$ such that for every $n\geq1$ there are $x_n,y_n\in[a,b]$ with

$$
|x_n-y_n|<1/n,\qquad |f(x_n)-f(y_n)|\geq\varepsilon_0.
$$

The [Bolzano-Weierstrass theorem](../../../../../../../bolzano-weierstrass-theorem.md), which states that every [bounded sequence](../../../../../../../bounded-sequence.md) of [real numbers](../../../../../../../real-number.md) has a [convergent subsequence](../../../../../../../convergent-subsequence.md), gives $x_{n_k}\to p$. The inequalities $a\leq x_{n_k}\leq b$ imply $p\in[a,b]$. By the [triangle inequality](../../../../../../../triangle-inequality.md),

$$
|y_{n_k}-p|\leq|y_{n_k}-x_{n_k}|+|x_{n_k}-p|\longrightarrow0.
$$

Since [continuous functions preserve convergent sequences](../../../../../../../continuous-functions-preserve-convergent-sequences.md), both $f(x_{n_k})$ and $f(y_{n_k})$ tend to $f(p)$. Their difference therefore tends to zero, contradicting its [absolute value](../../../../../../../absolute-value.md) being at least $\varepsilon_0$. This proves the [Heine-Cantor theorem](../../../../../../../heine-cantor-theorem.md) in the required setting: **$f$ has [uniform continuity](../../../../../../../uniform-continuity.md) on $[a,b]$.**

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
