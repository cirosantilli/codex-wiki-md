<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

Let $G(s)=\mathbb E[s^\xi]$ be the offspring [probability generating function](../../../../../probability-generating-function.md), and let $G_n(s)=\mathbb E[s^{Z_n}]$, for $0\leq s\leq1$. Given $Z_n=k$, the next generation is a sum of $k$ [independent](../../../../../independent-random-variables.md) offspring counts. Multiplication of their [probability generating functions](../../../../../probability-generating-function.md) gives

$$
\mathbb E[s^{Z_{n+1}}\mid Z_n=k]=G(s)^k.
$$

Taking [conditional expectation](../../../../../conditional-expectation.md) and then averaging proves

$$
\boxed{G_{n+1}(s)=G_n(G(s)),\qquad G_0(s)=s.}
$$

Thus $G_n$ is the $n$-fold composition of $G$ with itself. Induction makes this precise: it is true for $n=0$, and composing once more gives the next generation. In particular $G_n\circ G=G\circ G_n$, since both are the same iterated function. This is the generating-function recursion for a [Galton-Watson process](../../../../../galton-watson-process.md).

Write $m=\mathbb E Z_1=G'(1^-)$, initially assuming it is finite. The [law of total expectation](../../../../../law-of-total-expectation.md) gives

$$
\mathbb E[Z_{n+1}\mid Z_n]=mZ_n,
\qquad \mathbb E Z_{n+1}=m\mathbb E Z_n.
$$

Starting at one therefore yields $\boxed{\mathbb E Z_n=m^n}$, with the value at $n=0$ understood to be one even if $m=0$. Equivalently, differentiating the composition at one gives the same recurrence. If the offspring [expectation](../../../../../expected-value.md) is infinite, every positive generation has infinite [expectation](../../../../../expected-value.md): a positive chance of at least one parent remains at each finite generation, and conditional on any positive parent count the next expected count is infinite.

For a [Poisson branching process](../../../../../poisson-branching-process.md), $G(s)=e^{\lambda(s-1)}$. Extinction is absorbing because an empty generation has no parents, so extinction by generation $n$ is precisely $Z_n=0$. Hence $x_n=G_n(0)$. Using the composition in the order $G\circ G_n$ gives

$$
\boxed{x_{n+1}=e^{\lambda(x_n-1)},\qquad x_0=0.}
$$

For example $x_1=e^{-\lambda}$ is the chance of no offspring in the first generation. The recurrence includes the degenerate case $\lambda=0$, where extinction occurs in the first generation with certainty.

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
