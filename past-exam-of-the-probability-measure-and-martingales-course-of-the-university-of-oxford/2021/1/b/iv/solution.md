<h1 id="1/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The [L2-bounded martingale convergence theorem](../../../../../l2-bounded-martingale-convergence-theorem.md) states that a [martingale](../../../../../martingale-split.md) with $\sup_n\mathbb E|X_n|^2<\infty$ converges both [almost surely](../../../../../almost-sure-convergence.md) and with [convergence in L2](../../../../../convergence-in-l2.md) to a [square-integrable](../../../../../square-integrable-function.md) [random variable](../../../../../random-variable-split.md). Its hypotheses hold because $0<X_n<1$. Thus there is $X_\infty\in[0,1]$ [almost surely](../../../../../almost-sure-convergence.md) with both kinds of convergence. Alternatively, the [martingale convergence theorem](../../../../../martingale-convergence-theorem.md) gives the [almost sure convergence](../../../../../almost-sure-convergence.md), and the bound $|X_n-X_\infty|^2\leq1$ gives [convergence in L2](../../../../../convergence-in-l2.md) by the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md).[§4.4, Theorem 4.4.6, printed p. 237: the Lp martingale convergence theorem](../../../../../probability-theory-and-examples-fifth-edition-by-rick-durrett.md)

The calculation of the [conditional expectation](../../../../../conditional-expectation.md) of the square is especially informative. The [martingale](../../../../../martingale-split.md) property makes the cross term vanish in the square expansion, so

$$
\mathbb E[X_{n+1}^2\mid\mathcal F_n]
=X_n^2+\tfrac14X_n(1-X_n).
$$

Subtracting this from $\mathbb E[X_{n+1}\mid\mathcal F_n]=X_n$ gives

$$
\mathbb E[X_{n+1}(1-X_{n+1})\mid\mathcal F_n]
=\tfrac34X_n(1-X_n).
$$

Taking [expected values](../../../../../expected-value-split.md) and iterating proves

$$
\mathbb E[X_n(1-X_n)]=x(1-x)(3/4)^n.
$$

By [bounded convergence theorem](../../../../../bounded-convergence-theorem.md), $\mathbb E[X_\infty(1-X_\infty)]=0$. The [random variable](../../../../../random-variable-split.md) inside this [expected value](../../../../../expected-value-split.md) is nonnegative, so it is zero [almost surely](../../../../../almost-sure-convergence.md); on $[0,1]$ this forces $X_\infty\in\{0,1\}$. Again by [bounded convergence theorem](../../../../../bounded-convergence-theorem.md), $\mathbb EX_\infty=\lim_n\mathbb EX_n=x$. Hence

$$
\boxed{X_\infty\sim\operatorname{Bernoulli}(x),\qquad
\mathbb P(X_\infty=1)=x,\quad\mathbb P(X_\infty=0)=1-x.}
$$

This is the [Bernoulli polarization martingale](../../../../../bernoulli-polarization-martingale.md) with update size $1/2$. It also has an exact [mean squared error](../../../../../mean-squared-error.md): the terminal representation $X_n=\mathbb E[X_\infty\mid\mathcal F_n]$ and the [equality case for conditional second moments](../../../../../equality-case-for-conditional-second-moments.md) give

$$
\mathbb E[(X_\infty-X_n)^2]
=\mathbb E[X_\infty^2]-\mathbb E[X_n^2]
=x(1-x)(3/4)^n.
$$

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
