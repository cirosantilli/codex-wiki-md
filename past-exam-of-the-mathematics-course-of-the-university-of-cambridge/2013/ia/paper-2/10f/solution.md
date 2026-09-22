<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

For the [probability generating function](../../../../../probability-generating-function.md) $G(t)=\mathbb E[t^X]$, differentiation gives

$$
\boxed{G'(1)=\mathbb E[X]=\mu,\qquad
G''(1)=\mathbb E[X(X-1)]=\sigma^2+\mu^2-\mu}.
$$

The second [derivative](../../../../../derivative.md) is a [factorial moment](../../../../../factorial-moment.md), not the raw [second moment](../../../../../second-moment.md).

In the [Galton-Watson process](../../../../../galton-watson-process.md), condition on $X_n=m$. The next generation is a sum of $m$ independent offspring counts, and so its conditional generating function is $G(t)^m$. Averaging over $X_n$ gives

$$
\boxed{G_{n+1}(t)=\mathbb E[G(t)^{X_n}]=G_n(G(t))}.
$$

The conditional mean is $m\mu$ and the [conditional variance](../../../../../conditional-variance.md) is $m\sigma^2$. Thus iterated [expectation](../../../../../expected-value.md) gives $\mathbb E[X_n]=\mu^n$ from one ancestor, and the [law of total variance](../../../../../law-of-total-variance.md) gives $v_{n+1}=\mu^2v_n+\sigma^2\mu^n$, $v_0=0$. Iterating yields the [branching-process generation moments](../../../../../mean-and-variance-of-a-galton-watson-generation.md)

$$
\boxed{v_n=\sigma^2\mu^{n-1}\sum_{j=0}^{n-1}\mu^j
=\sigma^2\frac{\mu^{n-1}(\mu^n-1)}{\mu-1}\quad(\mu\ne1,\ n\geq1)}.
$$

For the critical case $\mu=1$, the correct limiting value is $v_n=n\sigma^2$. If $\mu=0$, nonnegative offspring are zero almost surely, so every later generation has zero mean and [variance](../../../../../variance-split.md); handle this directly rather than use an ambiguous zero power. At generation zero the mean is one and [variance](../../../../../variance-split.md) zero.

The [branching-process extinction criterion](../../../../../branching-process-extinction-criterion.md) states that extinction [probability](../../../../../probability.md) is the smallest fixed point of $G$ in $[0,1]$: probabilities of extinction by successive generations are the iterates of $G$ from zero, increasing to that fixed point. Here the equation is $4q^3-7q+3=0$, factoring as $(q-1)(2q-1)(2q+3)=0$. The two admissible roots are $1/2$ and one, so

$$
\boxed{\mathbb P(\text{eventual extinction})=\frac12}.
$$

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
