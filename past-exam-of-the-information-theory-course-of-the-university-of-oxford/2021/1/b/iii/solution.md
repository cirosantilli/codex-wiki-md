<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**Reference-distribution ambiguity:** $\rho$ is not defined in the paper. If it is an arbitrary [probability mass function](../../../../../probability-mass-function.md), the printed inequality is false. For instance, choose $p=(1,0)$ and $\rho=(1/2,1/2)$. Every [empirical distribution](../../../../../type-information-theory.md) equals $p$, making the printed left side one [bit](../../../../../bit.md) and its right side zero. This is a counterexample for every $n\geq1$.

Under the consistent interpretation **$\rho=p$**, the preceding [leave-one-out identity for empirical distributions](../../../../../leave-one-out-identity-for-empirical-distributions.md) and [convexity of relative entropy in its first argument](../../../../../convexity-of-relative-entropy-in-its-first-argument.md) give, for every sample,

$$
D(\widehat p_{n+1}\|p)
\leq\frac1{n+1}\sum_{i=1}^{n+1}D(\widehat q_{n,i}\|p).
$$

Deleting any one observation from $n+1$ [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) leaves $n$ [independent](../../../../../independent-random-variables.md) observations with [probability mass function](../../../../../probability-mass-function.md) $p$. Consequently each $\widehat q_{n,i}$ has the same distribution as $\widehat p_n$. They need not be [independent](../../../../../independent-random-variables.md) of one another. Taking [expected values](../../../../../expected-value-split.md) and using [linearity of expectation](../../../../../linearity-of-expectation.md) therefore proves

$$
\boxed{\mathbb E D(\widehat p_{n+1}\|p)\leq\mathbb E D(\widehat p_n\|p).}
$$

Zero coordinates of $p$ are never sampled, [almost surely](../../../../../almost-sure-convergence.md), so the calculation can be restricted to its [probability support](../../../../../support-of-a-probability-distribution.md). In particular the [expected values](../../../../../expected-value-split.md) are finite on this [finite alphabet](../../../../../finite-alphabet.md).

The discrepancy cannot be removed by silently choosing any fixed reference. Whenever $\rho$ is positive on the [probability support](../../../../../support-of-a-probability-distribution.md) of $p$, direct subtraction and $\mathbb E\widehat p_n=p$ give the [expected relative entropy decomposition](../../../../../expected-relative-entropy-decomposition.md)

$$
\mathbb E D(\widehat p_n\|\rho)=\mathbb E D(\widehat p_n\|p)+D(p\|\rho).
$$

Thus the valid arbitrary-reference version has $\rho$ on _both_ sides; the printed mixed-reference version has an additional term whose sign prevents the proposed conclusion.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the information theory course of the University of Oxford](../../../../split.md)
6. [Information theory course of the University of Oxford](../../../../../information-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
