<h1 id="7/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $M=\max_iX_i$. For an observed sample in the nonnegative orthant, the [likelihood function](../../../../../../../likelihood-function.md) under the [uniform distribution](../../../../../../../continuous-uniform-distribution.md) is

$$
L(\theta)=\theta^{-n}\mathbf1_{\{\theta\ge M\}},\qquad\theta>0.
$$

It is zero for $\theta<M$, and decreases with $\theta$ on $[M,\infty)$. Thus the [maximum likelihood estimation](../../../../../../../maximum-likelihood-estimation-split.md) problem is solved at the smallest admissible value:

$$
\boxed{\widehat\theta=M=\max_{1\le i\le n}X_i.}
$$

Under the model $M>0$ with [probability](../../../../../../../probability.md) one. The all-zero sample is a null event on which the [likelihood function](../../../../../../../likelihood-function.md) has no finite maximizer in the parameter space $\theta>0$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
