<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $B$ and $U$ are [independent random variables](../../../../../independent-random-variables.md), conditioning on the [Bernoulli random variable](../../../../../bernoulli-distribution.md) $B$ gives

$$
\boxed{M_Z(t)=(1-p)+pM_U(t)=1-p+p\frac{\sinh t}{t},}
$$

with the continuous value $M_Z(0)=1$. Indeed $Z=0$ when $B=0$, while the conditional [probability distribution](../../../../../probability-distribution-split.md) of $Z$ given $B=1$ is the original [uniform distribution](../../../../../continuous-uniform-distribution.md).

Under the literal assumptions alone, the [law of total expectation](../../../../../law-of-total-expectation.md) gives only

$$
M_Z(t)=1-p+p\mathbb E[e^{tU}\mid B=1].
$$

This is not determined by $M_U$ and $p$. For an explicit counterexample, put $p=1/2$ and $B=\mathbf1_{\{U>0\}}$. Then $B$ has the required [Bernoulli distribution](../../../../../bernoulli-distribution.md), but

$$
M_Z(t)=\frac12+\frac12\int_0^1e^{tu}\,du=\frac12+\frac{e^t-1}{2t}\quad(t\ne0),
$$

which differs from the independent-case formula.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
