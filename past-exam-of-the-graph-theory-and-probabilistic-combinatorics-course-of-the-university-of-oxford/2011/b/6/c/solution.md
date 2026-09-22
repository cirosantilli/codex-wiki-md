<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First take $0<p<1$ and $kp>1$. Part (a) gives an [extinction](../../../../../extinction.md) [probability](../../../../../probability.md) $\eta\in(0,1)$. Write $p_j=\mathbb P(Z=j)$. Conditional on the ancestor having $j$ children, [extinction](../../../../../extinction.md) requires [extinction](../../../../../extinction.md) of all $j$ [independent](../../../../../independent-random-variables.md) descendant trees and has [probability](../../../../../probability.md) $\eta^j$. Bayes' rule therefore gives the conditional offspring law

$$
\widetilde p_j=\mathbb P(Z=j\mid\text{extinction})=p_j\eta^{j-1}.
$$

Its sum is $f(\eta)/\eta=1$. Conditional on [extinction](../../../../../extinction.md) of all descendant trees, those trees remain [independent](../../../../../independent-random-variables.md), each with its own extinction-conditioned law. Thus the entire conditioned process is a Galton–Watson process with offspring generating function

$$
\widetilde f(s)=\frac{f(\eta s)}\eta.
$$

For binomial offspring, using $\eta=(1-p+p\eta)^k$ gives

$$
\boxed{\widetilde Z\sim\operatorname{Bi}(k,\widetilde p),\qquad
\widetilde p=\frac{p\eta}{1-p+p\eta}.}
$$

Its [mean](../../../../../expected-value-split.md) is $k\widetilde p=f'(\eta)<1$. Indeed, $f(s)-s$ is [strictly convex](../../../../../strictly-convex-function.md) and has its two zeros at $\eta$ and one, so its [derivative](../../../../../derivative.md) at the first zero is strictly negative. This proves subcriticality directly from the generating function.

Let $T$ be [total progeny](../../../../../total-progeny-of-a-branching-process.md), taking value infinity on survival. Apply part (b) to the conditioned process. For some $c>0$,

$$
\boxed{1-\eta\leq\mathbb P(T>n)
=(1-\eta)+\eta\,\mathbb P(\widetilde T>n)
\leq1-\eta+\eta e^{-cn}.}
$$

Thus the unconditional tail tends to the positive survival [probability](../../../../../probability.md) $1-\eta$, with an exponentially small finite-extinction contribution. It does not decay to zero.

If $p=1$ and $kp>1$, [extinction](../../../../../extinction.md) has [probability](../../../../../probability.md) zero and conditioning on it does not specify a [probability](../../../../../probability.md) law. In that deterministic case [total progeny](../../../../../total-progeny-of-a-branching-process.md) is infinite and $\mathbb P(T>n)=1$ for every finite $n$.

The nondegenerate law above is the [binomial branching process conditioned on extinction](../../../../../binomial-branching-process-conditioned-on-extinction.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
