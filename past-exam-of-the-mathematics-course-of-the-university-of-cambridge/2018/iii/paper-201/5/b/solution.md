<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $a>0$, the [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) at the [first-passage time](../../../../../../first-passage-time.md) of $a$ gives the [Brownian running maximum](../../../../../../brownian-running-maximum.md) identity

$$
\mathbb P(S_t\geq a)=2\mathbb P(B_t\geq a)=2\left(1-\Phi\left(\frac a{\sqrt t}\right)\right),\qquad t>0,
$$

where $\Phi$ is the [distribution function](../../../../../../cumulative-distribution-function.md) of the standard [normal distribution](../../../../../../normal-distribution.md). Indeed, reflection pairs paths that have reached $a$ and end below $a$ with paths ending above $a$; $B_t$ has no atom at $a$.

As $t\to\infty$, this probability tends to one. The [events](../../../../../../event.md) $\{S_n\geq a\}$ increase with integer $n$, so with probability one the path reaches $a$ in finite time. Taking a countable intersection over positive integer $a$ gives

$$
\boxed{\mathbb P(S_\infty=\infty)=1.}
$$

Here $S_\infty=\sup_{s\geq0}B_s$. This also proves that every positive-level [Brownian first-passage time](../../../../../../brownian-first-passage-time.md) is finite [almost surely](../../../../../../almost-sure-convergence.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
