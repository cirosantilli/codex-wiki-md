<h1 id="1/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Separate a long future count from the early [Poisson arrival time](../../../../../poisson-arrival-time.md). Let $\mathcal F_t=\sigma(N_s:0\leq s\leq t)$ be the [natural filtration](../../../../../natural-filtration.md), and define

$$
A_n=\frac{N_{n^4}-N_{n^2}-(n^4-n^2)}{n^2},\qquad
B_n=\frac{\min(T_n,n^2)-n}{\sqrt n},\qquad
C_n=\frac{N_{n^2}-n^2}{n^2}.
$$

The truncated [Poisson arrival time](../../../../../poisson-arrival-time.md) in $B_n$ is $\mathcal F_{n^2}$-measurable. The [independent increments](../../../../../independent-increments.md) property makes $A_n$ independent of $\mathcal F_{n^2}$, and hence of $B_n$.

The numerator of $A_n$ is a centered [Poisson random variable](../../../../../poisson-distribution.md) of parameter $n^4-n^2$. Apply the [central limit theorem](../../../../../central-limit-theorem.md) to the $n^4-n^2$ unit-time increments, then use $\sqrt{n^4-n^2}/n^2\to1$ and [Slutsky's theorem](../../../../../slutsky-theorem.md). This proves $A_n\xrightarrow{\mathrm d}N(0,1)$. Also, [Markov's inequality](../../../../../markov-s-inequality.md) and $\mathbb ET_n=n$ give

$$
\mathbb P(T_n>n^2)\leq\frac1n\longrightarrow0.
$$

Thus $B_n$ equals $(T_n-n)/\sqrt n$ outside an event of vanishing [probability](../../../../../probability.md), so part (i) and [Slutsky's theorem](../../../../../slutsky-theorem.md) give $B_n\xrightarrow{\mathrm d}N(0,1)$. Exact [independence of random variables](../../../../../independent-random-variables.md) for each $n$ now gives the joint limit $(A_n,B_n)\xrightarrow{\mathrm d}(Z_1,Z_2)$ with independent [standard normal random variables](../../../../../standard-normal-random-variable.md).

Finally, $\mathbb EC_n=0$ and $\operatorname{Var}(C_n)=n^{-2}$, so [Chebyshev's inequality](../../../../../chebyshev-s-inequality.md) gives $C_n\to0$ in [probability](../../../../../probability.md). The first coordinate in the question is $A_n+C_n$. The second differs from $B_n$ only on $\{T_n>n^2\}$, and so its difference tends to zero in [probability](../../../../../probability.md). The vector version of [Slutsky's theorem](../../../../../slutsky-theorem.md) proves the required joint [convergence in distribution](../../../../../convergence-in-distribution.md). The boundary of $(-\infty,x]\times[y,\infty)$ has zero limiting [probability](../../../../../probability.md), since both [marginal distributions](../../../../../marginal-distribution.md) have [continuous](../../../../../continuous-function.md) [cumulative distribution functions](../../../../../cumulative-distribution-function.md). The [Portmanteau theorem](../../../../../portmanteau-theorem.md) therefore yields

$$
\boxed{\mathbb P\!\left(\frac{N_{n^4}-n^4}{n^2}\leq x,\frac{T_n-n}{\sqrt n}\geq y\right)\longrightarrow\Phi(x)\bigl(1-\Phi(y)\bigr).}
$$

This is $\mathbb P(Z_1\leq x,Z_2\geq y)$ by [independence of random variables](../../../../../independent-random-variables.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
