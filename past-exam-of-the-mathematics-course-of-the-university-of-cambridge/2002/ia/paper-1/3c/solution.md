<h1 id="3c/solution">Solution</h1>

↑ **Parent:** [3C](../3c.md)

The [limit of a sequence](../../../../../limit-of-a-sequence.md) of [real numbers](../../../../../real-number.md) is $a$ if, for every $\varepsilon>0$, there is an [integer](../../../../../integer.md) $N$ such that $n\ge N$ implies $|a_n-a|<\varepsilon$. It tends to positive infinity if, for every real $M$, there is an [integer](../../../../../integer.md) $N$ such that $n\ge N$ implies $a_n>M$.

If $a_n\to+\infty$, choose the latter threshold with $M=1/\varepsilon$. Then $a_n>1/\varepsilon>0$ eventually, so $|1/a_n|<\varepsilon$. Thus $1/a_n\to0$. **The converse is false:** $a_n=-n$ has reciprocal tending to zero and tends to negative infinity. The precise sign-free statement is given by [reciprocal limits and escape in absolute value](../../../../../reciprocal-limits-and-escape-in-absolute-value.md): $1/a_n\to0$ is equivalent to $|a_n|\to\infty$.

If $a_n\to a\ne0$, eventually $|a_n-a|<|a|/2$, and the [triangle inequality](../../../../../triangle-inequality.md) gives $|a_n|>|a|/2$. Consequently

$$
\left|\frac1{a_n}-\frac1a\right|
=\frac{|a_n-a|}{|a_n||a|}\le\frac{2|a_n-a|}{|a|^2}.
$$

Given $\varepsilon>0$, take $N$ large enough that $|a_n-a|<\min(|a|/2,\varepsilon|a|^2/2)$ for all $n\ge N$. This proves **$1/a_n\to1/a$** directly from the definition of the [limit of a sequence](../../../../../limit-of-a-sequence.md).

## ↑ Ancestors (11)

1. [3C](../3c.md)
2. [Section I](../section-i.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ia](../../split.md)
5. [2002](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
