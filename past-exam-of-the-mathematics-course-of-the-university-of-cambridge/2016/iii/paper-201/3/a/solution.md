<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mu=\mathbb E X_1$ and let the [cumulant-generating function](../../../../../../cumulant-generating-function.md) and its [Legendre transform](../../../../../../convex-conjugate.md) be

$$
\psi(\theta)=\log\mathbb E e^{\theta X_1},
\qquad I(x)=\sup_{\theta\in\mathbb R}\{\theta x-\psi(\theta)\}.
$$

Under the permitted assumption that $\psi$ is finite everywhere, the right-tail form of the [Cramér theorem](../../../../../../cramer-s-theorem.md) is, for $a\geq\mu$,

$$
\boxed{\lim_{n\to\infty}\frac1n\log\mathbb P(S_n\geq na)=-I(a),
\qquad I(a)=\sup_{\theta\geq0}\{\theta a-\psi(\theta)\}.}
$$

Use $\log0=-\infty$. The restriction to nonnegative parameters is valid on this side of the mean: convexity gives $\psi(\theta)\geq\mu\theta$, so negative parameters cannot improve the value zero available at $\theta=0$. For $a<\mu$, the right-tail probability tends to one by the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md), so its logarithmic rate is zero; it is not generally $-I(a)$.

The full [large deviation principle](../../../../../../large-deviation-principle.md) bounds probabilities of closed sets from above and open sets from below with rate $I$. For the displayed tail equality, a possible finite upper endpoint also needs attention. If $b=\operatorname{ess\,sup}X_1<\infty$, then at $a=b$ the event requires every summand to equal $b$; its probability is $\mathbb P(X_1=b)^n$, and $I(b)=-\log\mathbb P(X_1=b)$. The identity follows by taking $\theta\to\infty$ in $\mathbb E e^{\theta(X_1-b)}$. Above $b$, both sides have infinite rate. **The theorem describes exponential decay, including endpoints and impossible events.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
