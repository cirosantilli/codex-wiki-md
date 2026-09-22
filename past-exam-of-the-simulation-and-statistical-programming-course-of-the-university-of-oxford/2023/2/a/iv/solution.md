<h1 id="2/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use the same acceptance [indicator functions](../../../../../indicator-function.md) and set $K_n=\sum_{i=1}^nA_i$, $S_n=\sum_{i=1}^nA_i\phi(Y_i)$. The [rejection sampling](../../../../../rejection-sampling.md) estimator based on these $n$ proposals is the mean over the accepted observations:

$$
\boxed{\widehat\theta_n^{\mathrm{RS}}=\frac{S_n}{K_n}\quad(K_n>0).}
$$

For $K_n=0$, any fixed convention, such as zero, is harmless asymptotically. The $A_i$ are [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) with [Bernoulli distribution](../../../../../bernoulli-distribution.md) and success [probability](../../../../../probability.md) $1/M$, so the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) gives $K_n/n\to1/M$ [almost surely](../../../../../almost-sure-convergence.md). In particular $K_n>0$ eventually [almost surely](../../../../../almost-sure-convergence.md). The exact identity

$$
\boxed{\widehat\theta_n^{\mathrm{IS}}=\frac{MK_n}{n}\widehat\theta_n^{\mathrm{RS}}}
$$

then holds whenever $K_n>0$. Wherever $S_n\ne0$, it follows that

$$
\frac{\widehat\theta_n^{\mathrm{IS}}}{\widehat\theta_n^{\mathrm{RS}}}
=\frac{MK_n}{n}\longrightarrow1\quad\text{almost surely}.
$$

A qualification is missing from the printed claim: the quotient must be defined eventually. A convenient sufficient assumption is $\mathbb E_p|\phi|<\infty$ and $\theta\ne0$. Indeed, another application of the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) gives $S_n/n\to\theta/M$, ensuring that $S_n$ is eventually nonzero. This proves the stated quotient limit under that assumption.

As printed, the assertion is false as a universally defined quotient. For example, $\phi\equiv0$ makes both estimates zero for every $n$. Even excluding that example is insufficient: take $p=q$ to be the [uniform distribution](../../../../../continuous-uniform-distribution.md) on $(0,1)$, $M=1$, and $\phi(y)=1$ for $y<1/2$ and $-1$ otherwise. Then $S_n$ is a [simple symmetric random walk](../../../../../simple-symmetric-random-walk.md), which returns to zero infinitely often [almost surely](../../../../../almost-sure-convergence.md), leaving the quotient undefined infinitely often.

With integrability but no assumption $\theta\ne0$, the exact multiplicative identity remains valid, and both estimates converge to $\theta$ [almost surely](../../../../../almost-sure-convergence.md). In particular $\widehat\theta_n^{\mathrm{IS}}-\widehat\theta_n^{\mathrm{RS}}\to0$ [almost surely](../../../../../almost-sure-convergence.md). One may alternatively define the quotient's removable $0/0$ cases as $MK_n/n$; that explicitly extended quantity always converges to one. These are valid repairs of the source's unrestricted statement.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
