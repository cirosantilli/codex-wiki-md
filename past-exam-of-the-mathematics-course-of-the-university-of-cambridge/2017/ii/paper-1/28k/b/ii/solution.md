<h1 id="28k/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Condition on $X=k$. For $0<k<n$, the posterior expected loss is a strictly convex quadratic in the decision $d$. Its minimizer is

$$
d=\frac{\mathbb E[1/(1-p)\mid k]}{\mathbb E[1/p\mid k]+\mathbb E[1/(1-p)\mid k]}.
$$

The beta density gives $\mathbb E[1/p\mid k]=(n+1)/k$ and $\mathbb E[1/(1-p)\mid k]=(n+1)/(n-k)$, so $d=k/n$. If $k=0$, every $d\ne0$ has infinite posterior expected loss because of the nonintegrable $d^2/p$ term near zero, whereas $d=0$ has finite loss [expectation](../../../../../../../expected-value.md). The analogous argument at $k=n$ forces $d=1$. Hence the [Bayes estimator](../../../../../../../bayes-estimator.md) is

$$
\boxed{\delta_B(X)=X/n,\qquad R(p,\delta_B)=1/n\quad(0<p<1)}.
$$

Indeed $X/n$ is unbiased and has [variance](../../../../../../../variance-split.md) $p(1-p)/n$, which cancels the loss denominator. Its uniform-prior [Bayes risk](../../../../../../../bayes-risk.md) is $1/n$.

The printed loss is undefined at $p=0,1$, despite the stated closed parameter interval. A convention is necessary there. The natural extended loss assigns zero to the correct endpoint decision and infinity to an incorrect one; it gives endpoint risks zero for $X/n$. Alternatively a continuous extension of this estimator's risk gives endpoint values $1/n$. The interior result and the minimax value below are unchanged by either convention, and a [uniform prior](../../../../../../../uniform-prior.md) gives the endpoints measure zero. We do not identify an undefined $0/0$ with a value without specifying this choice.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [28K](../../../28k.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
