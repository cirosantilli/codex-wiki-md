<h1 id="12d/solution">Solution</h1>

↑ **Parent:** [12D](../12d.md)

A [simple hypothesis](../../../../../simple-hypothesis.md) specifies a single probability law, with no unknown parameter remaining. For a possibly randomized [hypothesis test](../../../../../statistical-hypothesis-test.md), let $\varphi(x)\in[0,1]$ be its conditional rejection probability. Its [test size](../../../../../size-of-a-statistical-test.md) is $E_0\varphi(X)$ and its [statistical power](../../../../../statistical-power.md) against the specified alternative is $E_1\varphi(X)$.

The [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) states that for two densities $f_0,f_1$ with respect to a common measure, a [likelihood-ratio test](../../../../../likelihood-ratio-test.md) rejecting when $f_1/f_0>k$, accepting when it is below $k$, and randomizing on equality to obtain size $\alpha$, maximizes power among all tests of size at most $\alpha$.

Here the [likelihood ratio](../../../../../likelihood-ratio.md) is

$$
\Lambda(x)=\frac{\sqrt{2\pi}}4\exp\left(\frac{x^2-|x|}{2}\right).
$$

Writing $r=|x|$, its logarithm apart from the constant is $(r^2-r)/2$. This decreases until $r=1/2$ and then increases. In particular it is nonpositive for $0\leq r\leq1$ and positive for $r>1$. The supplied normal-tail value and $\alpha<1/4$ imply that the quantile $t$ defined by $2[1-\Phi(t)]=\alpha$ satisfies $t>1$. Hence the threshold $\Lambda(t)$ is above every central value on $r\leq1$; outside that interval the ratio is strictly increasing. The [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) therefore selects precisely the two tails:

$$
\boxed{\text{reject }H_0\text{ if }|X|>t,\qquad \Phi(t)=1-\alpha/2}.
$$

The equality boundary has probability zero under both continuous laws, so no randomization is needed. Under the alternative density, the [statistical power](../../../../../statistical-power.md) is

$$
\boxed{\int_{|x|>t}\frac14e^{-|x|/2}\,dx=e^{-t/2}}.
$$

The central dip in the [likelihood ratio](../../../../../likelihood-ratio.md) is why checking the threshold against the entire central region, rather than assuming monotonicity in $|x|$ everywhere, is necessary.

## ↑ Ancestors (10)

1. [12D](../12d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
