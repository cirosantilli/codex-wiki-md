<h1 id="6h/solution">Solution</h1>

↑ **Parent:** [6H](../6h.md)

The [Rao-Blackwell theorem](../../../../../rao-blackwell-theorem.md) says that if $U$ is an estimator with finite second moment and $T$ is a [sufficient statistic](../../../../../sufficient-statistic.md), then

$$
U^*=\mathbb E[U\mid T]
$$

has the same expectation as $U$ and satisfies

$$
\operatorname{Var}(U^*)\leq\operatorname{Var}(U),
$$

with equality only when $U$ is already a function of $T$ almost surely.

Here $\widehat\theta=\mathbf1_{\{X_1=1\}}$ is unbiased because

$$
\mathbb E\widehat\theta
=\mathbb P(X_1=1)=p(1-p)=\theta.
$$

Conditional on $T=t$, every weak composition $(x_1,\ldots,x_n)$ of $t$ has the same probability $p^n(1-p)^t$. There are

$$
\binom{t+n-1}{n-1}
$$

such compositions. For $t\geq1$, those with $x_1=1$ correspond to weak compositions of $t-1$ into $n-1$ parts, of which there are

$$
\binom{t+n-3}{n-2}.
$$

The Rao-Blackwell estimator is therefore

$$
\boxed{
\widehat\theta^*(T)=
\begin{cases}
\displaystyle
\frac{(n-1)T}{(T+n-1)(T+n-2)},&T\geq1,\\[6pt]
0,&T=0.
\end{cases}}
$$

For $n\geq2$ and $0<p<1$, $\widehat\theta$ is not determined by $T$; for example, conditional on $T=1$, the sole failure can occur in any coordinate. The variance inequality is consequently strict:

$$
\boxed{\operatorname{Var}(\widehat\theta^*)<
\operatorname{Var}(\widehat\theta)}.
$$

## ↑ Ancestors (10)

1. [6H](../6h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
