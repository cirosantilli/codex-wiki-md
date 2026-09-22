<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For an $n$-dimensional [random vector](../../../../../random-vector.md) with a density and finite [differential entropy](../../../../../differential-entropy.md) in bits, define its [entropy power](../../../../../entropy-power.md) by $N(X)=(2\pi e)^{-1}2^{2h(X)/n}$. The [entropy power inequality](../../../../../entropy-power-inequality.md) states that for independent such [random vectors](../../../../../random-vector.md),

$$
\boxed{N(X+Y)\geq N(X)+N(Y),\quad\text{equivalently}\quad
2^{2h(X+Y)/n}\geq2^{2h(X)/n}+2^{2h(Y)/n}.}
$$

Here the sum's [differential entropy](../../../../../differential-entropy.md) must be defined, with $+\infty$ permitted.

Since $g'(x)>0$, the [mean value theorem](../../../../../mean-value-theorem.md) makes $g$ strictly increasing. Its image is an interval $I$, and its inverse on $I$ has [derivative](../../../../../derivative.md) $1/g'(g^{-1}(y))$. The density [change of variables](../../../../../change-of-variables-formula.md) gives

$$
p_{g(X)}(y)=
\begin{cases}
\dfrac{p_X(g^{-1}(y))}{g'(g^{-1}(y))},&y\in I,\\
0,&y\notin I.
\end{cases}
$$

This does not require $g$ to map onto all of $\mathbb R$. Taking logarithms at $y=g(X)$ and then [expected values](../../../../../expected-value.md) proves the [differential entropy under an increasing transformation](../../../../../differential-entropy-under-an-increasing-transformation.md):

$$
\boxed{h(g(X))=-\mathbb E\log_2p_X(X)+\mathbb E\log_2g'(X)
=h(X)+\mathbb E\log_2g'(X).}
$$

The two finite expectations in the assumptions justify splitting the expectation and imply that the transformed [differential entropy](../../../../../differential-entropy.md) is finite.

To derive the product inequality, assume that $h(Y_i)$ and $\mu_i=\mathbb E\log_2Y_i$ are finite and that the [differential entropy](../../../../../differential-entropy.md) of the logarithmic sum is defined. Set $Z_i=\ln Y_i$, using natural logarithms for this transformation while measuring [differential entropy](../../../../../differential-entropy.md) in bits. On the positive half-line the [derivative](../../../../../derivative.md) of $\ln y$ is $1/y$, so the same density argument gives

$$
h(Z_i)=h(Y_i)-\mu_i.
$$

The $Z_i$ are [independent random variables](../../../../../independent-random-variables.md), and the one-dimensional [entropy power inequality](../../../../../entropy-power-inequality.md) yields

$$
2^{2h(Z_1+Z_2)}\geq2^{2h(Z_1)}+2^{2h(Z_2)}.
$$

Since $Y_1Y_2=\exp(Z_1+Z_2)$, another [change of variables](../../../../../change-of-variables-formula.md) gives

$$
h(Y_1Y_2)=h(Z_1+Z_2)+\mathbb E\log_2(Y_1Y_2)
=h(Z_1+Z_2)+\mu_1+\mu_2.
$$

Multiplying the [entropy power inequality](../../../../../entropy-power-inequality.md) by $2^{2(\mu_1+\mu_2)}$ proves the [multiplicative entropy power inequality](../../../../../multiplicative-entropy-power-inequality.md):

$$
\boxed{2^{2h(Y_1Y_2)}
\geq 2^{2\mu_2}2^{2h(Y_1)}+2^{2\mu_1}2^{2h(Y_2)},\qquad
\alpha_1=2^{2\mu_2},\quad\alpha_2=2^{2\mu_1}.}
$$

The printed positivity and density assumptions alone do not ensure that the quantities in this last formula exist. For a concrete example, let $T$ have the standard [Cauchy distribution](../../../../../cauchy-distribution.md) and put $Y=e^T$. Then

$$
p_Y(y)=\frac{1}{\pi y(1+(\ln y)^2)},\qquad y>0,
$$

is a density, but $\mathbb E\log_2Y=(\log_2e)\mathbb ET$ is undefined because its positive and negative parts both diverge. Two independent copies satisfy the printed hypotheses but leave $\alpha_1,\alpha_2$ undefined. The product inequality therefore needs the finiteness or well-definedness conditions used above.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
