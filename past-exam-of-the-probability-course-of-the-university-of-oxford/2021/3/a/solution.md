<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The history $\sigma(S_0,\ldots,S_n)$ is contained in $\sigma(Y_1,\ldots,Y_n)$. The increment $Y_{n+1}$ is independent of this history by the given [independence of random variables](../../../../independent-random-variables.md). Therefore

$$
\mathbb P(S_{n+1}=j\mid S_0,\ldots,S_n)
=\mathbb P(Y_{n+1}=j-S_n\mid S_0,\ldots,S_n)
=p\mathbf1_{\{j=S_n+a\}}+q\mathbf1_{\{j=S_n-b\}}.
$$

This depends only on the current state and not on time. It is precisely the [time-homogeneous Markov property](../../../../time-homogeneous-markov-property.md), so $S_n$ is a [Markov chain](../../../../markov-chain-split.md) with [transition probabilities](../../../../transition-probability.md)

$$
\boxed{p_{i,j}=\begin{cases}b/(a+b),&j=i+a,\\a/(a+b),&j=i-b,\\0,&\text{otherwise},\end{cases}\qquad i,j\in\mathbb Z.}
$$

The conditional identity is an identity that holds [almost surely](../../../../almost-sure-convergence.md); histories of zero [probability](../../../../probability.md) require no division by their [probabilities](../../../../probability.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the probability course of the University of Oxford](../../../split.md)
5. [Probability course of the University of Oxford](../../../../probability-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
