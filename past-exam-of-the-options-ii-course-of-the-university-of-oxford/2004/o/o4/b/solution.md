<h1 id="o/o4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For any fixed $p>1/4$ below 1, the ratio to the null is

$$
\frac{f_p(y)}{f_{1/4}(y)}=[4(1-p)/3]^5\left(\frac{3p}{1-p}\right)^y.
$$

It increases with $y$. Its ordering is therefore the same for every such alternative, while the size is determined only by the null. The very same rule, **reject when $Y\geq4$**, is most powerful against each alternative and hence is a [uniformly most powerful test](../../../../../uniformly-most-powerful-test.md). At $p=1$ its power is 1, also optimal.

More generally, for $0<p_0<1$, the [binomial likelihood](../../../../../binomial-likelihood.md) ratio against any $p>p_0$ increases with $y$. Choose an integer cutoff $c$ so that

$$
\mathbb P_{p_0}(Y>c)\leq\alpha\leq\mathbb P_{p_0}(Y\geq c),
$$

and reject for $Y>c$, randomize with probability

$$
\boxed{\gamma=\frac{\alpha-\mathbb P_{p_0}(Y>c)}{\mathbb P_{p_0}(Y=c)}}
$$

when $Y=c$, and accept below. This gives exact size $\alpha$ and is a [uniformly most powerful test](../../../../../uniformly-most-powerful-test.md) for every positive integer $n$. Exact prescribed size may require this boundary randomization; a deterministic cutoff alone need not attain it. For $p_0=0$, reject all $Y>0$ and reject at $Y=0$ with probability $\alpha$, which is likewise optimal. At $p_0=1$ the stated one-sided alternative is empty. The cutoff generally depends on $p_0,n,\alpha$; there is no claim that one fixed cutoff serves every null parameter.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [O4](../../o4.md)
3. [O](../../../o.md)
4. [2004](../../../../2004-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
