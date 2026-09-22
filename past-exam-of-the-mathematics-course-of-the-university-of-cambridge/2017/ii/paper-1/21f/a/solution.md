<h1 id="21f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The continuous [dual space](../../../../../../dual-space.md) $X^*$ consists of all bounded real [linear functionals](../../../../../../linear-functional.md) on $X$, with [operator norm](../../../../../../operator-norm.md) $\|f\|=\sup_{\|x\|\le1}|f(x)|$. Let $(f_n)$ be Cauchy in this [norm](../../../../../../norm.md). For each $x$, $|f_n(x)-f_m(x)|\le\|f_n-f_m\|\|x\|$, so $f_n(x)$ converges in $\mathbb R$; define its limit to be $f(x)$.

Pointwise limits of the linear identities show that $f$ is linear. The [sequence](../../../../../../sequence.md) of [norms](../../../../../../norm.md) is bounded, say by $M$, so $|f(x)|\le M\|x\|$ and $f\in X^*$. Given $\varepsilon>0$, choose $N$ so that $\|f_n-f_m\|\le\varepsilon$ for all $m,n\ge N$. Holding $n$ fixed and taking the pointwise limit in $m$ gives $|f_n(x)-f(x)|\le\varepsilon\|x\|$ for all $x$. Thus $\|f_n-f\|\le\varepsilon$, proving

$$
\boxed{X^*\text{ is a Banach space}}.
$$

Completeness of $X$ is not needed; completeness of the scalar [field](../../../../../../field.md) supplies the pointwise limit.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [21F](../../21f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
