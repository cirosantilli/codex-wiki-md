<h1 id="10d/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**Yes.** The arbitrary variable-lag condition forces the [Cauchy sequence](../../../../../../cauchy-sequence.md) property. Suppose otherwise. Then some $\varepsilon_0>0$ has the property that, for every $N$, there exist $p,q\geq N$ with $|a_p-a_q|\geq\varepsilon_0$. In particular, for each $n$, choose such $p,q\geq n$. By the [triangle inequality](../../../../../../triangle-inequality.md), at least one satisfies $|a_p-a_n|\geq\varepsilon_0/2$ or $|a_q-a_n|\geq\varepsilon_0/2$. That index must be strictly greater than $n$, since the difference at $n$ itself is zero.

It follows that the following positive integer is defined for every $n$:

$$
f(n)=\min\{k\geq1:\ |a_{n+k}-a_n|\geq\varepsilon_0/2\}.
$$

For this particular function, $|a_{n+f(n)}-a_n|\geq\varepsilon_0/2$ for every $n$, contradicting the assumed limit zero. Therefore $(a_n)$ is a [Cauchy sequence](../../../../../../cauchy-sequence.md), and the [completeness of the real numbers](../../../../../../completeness-of-the-real-numbers.md) proves **it converges to a finite real limit**. This is [convergence from arbitrary variable-lag increments](../../../../../../convergence-from-arbitrary-variable-lag-increments.md); the quantifier over every function is much stronger than the fixed-lag condition in the previous part.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [10D](../../10d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
