<h1 id="12f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Chebyshev inequality](../../../../../../chebyshev-inequality.md) states that for a [random variable](../../../../../../random-variable-split.md) $Z$ with finite [variance](../../../../../../variance-split.md) and $a>0$,

$$
\mathbb P\bigl(|Z-\mathbb E[Z]|\geq a\bigr)\leq\frac{\operatorname{Var}(Z)}{a^2}.
$$

Write $\mu_n=\mathbb E[T]$. The ratio in the hypothesis presupposes $\mu_n>0$ for all sufficiently large $n$. On the event $T=0$, the deviation from the mean equals $\mu_n$. Thus the [Chebyshev inequality](../../../../../../chebyshev-inequality.md) with $a=\mu_n$ gives

$$
\boxed{\mathbb P(T=0)\leq\frac{\operatorname{Var}(T)}{\mathbb E[T]^2}\longrightarrow0.}
$$

This is the [second moment method](../../../../../../second-moment-method.md). It uses only the stipulated relative [variance](../../../../../../variance-split.md) bound; no assumption that triangle indicators are independent is needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
