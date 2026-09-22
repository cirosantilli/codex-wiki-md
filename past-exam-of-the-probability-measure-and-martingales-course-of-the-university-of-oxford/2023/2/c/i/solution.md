<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Each $Z_n$ is a bounded [Borel measurable function](../../../../../borel-measurable-function.md) of $X_n$, including the specified value at $X_n=1$. Therefore $(Z_n)$ is an [adapted process](../../../../../adapted-process.md) for $(\mathcal F_n)$ and consists of [integrable random variables](../../../../../integrable-random-variable.md).

Fix an [atom of a sigma-algebra](../../../../../atom-of-a-sigma-algebra.md) in $\mathcal F_n$ with positive [probability](../../../../../probability.md), corresponding to the [dyadic interval](../../../../../dyadic-interval.md) $[u,u+\delta)$, with $\delta=2^{-n}$. By the [uniform distribution](../../../../../continuous-uniform-distribution.md), each half has [conditional probability](../../../../../conditional-probability.md) $1/2$. The [conditional expectation](../../../../../conditional-expectation.md) of $Z_{n+1}$ on that atom is therefore

$$
\begin{aligned}
\frac12\bigl[2^{n+1}(f(u+\delta/2)-f(u))
+2^{n+1}(f(u+\delta)-f(u+\delta/2))\bigr]
&=2^n(f(u+\delta)-f(u))\\
&=Z_n.
\end{aligned}
$$

The middle values cancel. On the zero-[probability](../../../../../probability.md) atom the [conditional expectation](../../../../../conditional-expectation.md) can be chosen as zero, agreeing with our version of $Z_n$. Hence

$$
\boxed{\mathbb E[Z_{n+1}\mid\mathcal F_n]=Z_n\quad\text{almost surely},}
$$

so $(Z_n)$ is a [martingale](../../../../../martingale-split.md). This is the [dyadic slope martingale](../../../../../dyadic-slope-martingale.md) associated with the [Lipschitz function](../../../../../lipschitz-continuity.md) $f$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
