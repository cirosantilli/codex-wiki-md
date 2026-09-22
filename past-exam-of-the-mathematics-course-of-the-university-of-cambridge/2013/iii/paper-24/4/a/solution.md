<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [version of a stochastic process](../../../../../../modification-of-a-stochastic-process.md) means a [stochastic process](../../../../../../stochastic-process-split.md) on the same probability space such that, for every fixed $t$,

$$
\mathbb P(X_t=Y_t)=1.
$$

The exceptional [null set](../../../../../../null-set.md) may depend on $t$. [Indistinguishability of stochastic processes](../../../../../../indistinguishability-of-stochastic-processes.md) means that there is one [null set](../../../../../../null-set.md) outside which $X_t=Y_t$ for all $t\geq0$ simultaneously.

For an example separating the definitions, let $U$ have [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $(0,1)$, and set

$$
X_t=0,\qquad Y_t=\mathbf1_{\{t=U\}},\qquad t\geq0.
$$

For every fixed $t$, $\mathbb P(U=t)=0$, so $Y$ is a [version of a stochastic process](../../../../../../modification-of-a-stochastic-process.md) with original [stochastic process](../../../../../../stochastic-process-split.md) $X$. But for every sample outcome the [stochastic processes](../../../../../../stochastic-process-split.md) differ at its time $t=U$. Hence

$$
\boxed{\mathbb P(X_t=Y_t\text{ for every }t\geq0)=0.}
$$

The spike path of $Y$ is not [right-continuous](../../../../../../right-continuous-function.md) at $U$, which explains why the next part's regularity assumption rules out this example.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
