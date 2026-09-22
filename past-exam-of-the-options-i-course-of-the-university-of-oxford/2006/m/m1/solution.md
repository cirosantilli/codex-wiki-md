<h1 id="m/m1/solution">Solution</h1>

↑ **Parent:** [M1](../m1.md)

[Convergence in probability](../../../../convergence-in-probability.md) means that for every $\varepsilon>0$, $\mathbb P(|X_n-X|\geq\varepsilon)\to0$. The use of $>$ instead of $\geq$ gives the equivalent definition by replacing $\varepsilon$ with a smaller positive number.

For $Y\geq0$, the pointwise inequality $Y\geq a\mathbf1_{\{Y\geq a\}}$ gives, on taking [expected values](../../../../expected-value-split.md), [Markov's inequality](../../../../markov-s-inequality.md)

$$
\mathbb P(Y\geq a)\leq\frac{\mathbb EY}{a}.
$$

This also holds if the expectation is infinite, though the resulting bound is then uninformative. Apply it to $Y=(X-\mu)^2$ with threshold $\varepsilon^2$ to obtain [Chebyshev's inequality](../../../../chebyshev-s-inequality.md):

$$
\mathbb P(|X-\mu|\geq\varepsilon)\leq\sigma^2/\varepsilon^2.
$$

Set $S_n=n^{-1}\sum_{i=1}^n(Z_i-\mathbb EZ_i)$. Its mean is zero. [Independence](../../../../independent-random-variables.md) eliminates cross covariances, and boundedness gives $\operatorname{Var}(Z_i)\leq\mathbb EZ_i^2\leq1$. Hence

$$
\operatorname{Var}(S_n)=\frac1{n^2}\sum_{i=1}^n\operatorname{Var}(Z_i)\leq\frac1n,
\qquad\mathbb P(|S_n|\geq\varepsilon)\leq\frac1{n\varepsilon^2}\to0.
$$

Thus $\boxed{S_n\to0\text{ in probability}}$. Identical distributions were never needed.

## ↑ Ancestors (12)

1. [M1](../m1.md)
2. [M](../../m.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
