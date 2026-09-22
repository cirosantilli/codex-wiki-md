<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [sample maximum](../../../../../sample-maximum.md) has [cumulative distribution function](../../../../../cumulative-distribution-function.md)

$$
F_{M_n}(x)=\mathbb P(X_1\leq x,\ldots,X_n\leq x)
=\begin{cases}0,&x<0,\\x^n,&0\leq x\leq1,\\1,&x>1.\end{cases}
$$

The product $x^n$ follows from [independence of random variables](../../../../../independent-random-variables.md) and the [continuous uniform distribution](../../../../../continuous-uniform-distribution.md) of each observation. For every $x<1$, this [cumulative distribution function](../../../../../cumulative-distribution-function.md) tends to zero; for $x>1$ it equals one. These are exactly the values of the [cumulative distribution function](../../../../../cumulative-distribution-function.md) of the constant [random variable](../../../../../random-variable-split.md) $1$ at its continuity points. Therefore, by the definition of [convergence in distribution](../../../../../convergence-in-distribution.md),

$$
\boxed{M_n\xrightarrow{\mathrm d}1.}
$$

At $x=1$ the limiting [cumulative distribution function](../../../../../cumulative-distribution-function.md) is discontinuous, so the definition does not require checking that point, although $F_{M_n}(1)=1$ also holds.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
