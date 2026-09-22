<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Mix the conditional [Poisson distribution](../../../../../../poisson-distribution.md) over the rate-$\nu$ [exponential distribution](../../../../../../exponential-distribution.md) intensity. The [Gamma integral](../../../../../../gamma-integral.md) gives

$$
\mathbb P(N=j)=\int_0^\infty\frac{e^{-\lambda}\lambda^j}{j!}\nu e^{-\nu\lambda}\,d\lambda
=\frac{\nu}{(1+\nu)^{j+1}}=pq^j,
$$

where $p=\nu/(1+\nu)$ and $q=1/(1+\nu)$. Thus the annual [claim count](../../../../../../claim-count.md) has the zero-based [geometric distribution](../../../../../../geometric-distribution.md), with probabilities $\mathbb P(N=0)=p$, $\mathbb P(N=1)=pq$ and $\mathbb P(N\ge2)=q^2$.

For the intended [Markov chain](../../../../../../markov-chain.md) calculation, take these annual counts to be independent. Order the states by discounts $0,\alpha,\beta$. From either of the first two states, a positive count returns the policy to zero, while a zero count raises it by one level. From the top, two or more claims send it to zero, exactly one sends it to $\alpha$, and no claim keeps it at $\beta$. Hence the [transition matrix](../../../../../../stochastic-matrix.md) is

$$
\boxed{P=\begin{pmatrix}q&p&0\\q&0&p\\q^2&pq&p\end{pmatrix}.}
$$

Write its [stationary distribution](../../../../../../stationary-distribution.md) as $(\pi_0,\pi_\alpha,\pi_\beta)$. The final two balance equations give $q\pi_\beta=p\pi_\alpha$ and $\pi_\alpha=p\pi_0+pq\pi_\beta$. It follows that $\pi_\alpha=p\pi_0/[q(1+p)]$ and $\pi_\beta=p^2\pi_0/[q^2(1+p)]$. Normalizing yields the [three-level discount equilibrium with geometric annual counts](../../../../../../three-level-discount-equilibrium-with-geometric-annual-counts.md):

$$
\boxed{(\pi_0,\pi_\alpha,\pi_\beta)=\frac{(q^2(1+p),pq,p^2)}{1-p^2q}.}
$$

The [Markov chain](../../../../../../markov-chain.md) is irreducible for $0<p,q<1$ and has a self-loop, so it is aperiodic and this equilibrium is the limiting distribution. Weighting the three premiums $c,c(1-\alpha),c(1-\beta)$ gives

$$
\boxed{\mathbb E[\text{stationary premium}]=c\left[1-\frac{\alpha pq+\beta p^2}{1-p^2q}\right].}
$$

There is a necessary qualification to the temporal model: the one-year mixture alone does not specify independence between years. A [persistent claim intensity can destroy the discount Markov property](../../../../../../persistent-claim-intensity-can-destroy-the-discount-markov-property.md). If one fixed $\Lambda$ is drawn for the policyholder and annual counts are conditionally independent given it, then histories $0,\alpha,\beta,\beta$ and $0,0,\alpha,\beta$ both end at the top after three years but give different next-year no-claim probabilities. The first history is three zero counts, so its posterior intensity has exponential rate $\nu+3$ and next no-claim probability $(\nu+3)/(\nu+4)$. The second is a positive count followed by two zero counts; its posterior density is proportional to $(1-e^{-\lambda})e^{-(\nu+2)\lambda}$, giving next no-claim probability $(\nu+2)/(\nu+4)$. Thus the displayed matrix and premium require independent annual marginal sampling, for example a fresh intensity each year. They are not valid for a persistent unobserved policy intensity without conditioning on that intensity.

Under the persistent-intensity interpretation, one can instead condition on $\lambda$. Put $a_0=e^{-\lambda}$ and $b_1=\lambda e^{-\lambda}$. The conditional [transition matrix](../../../../../../stochastic-matrix.md) has rows $(1-a_0,a_0,0)$, $(1-a_0,0,a_0)$ and $(1-a_0-b_1,b_1,a_0)$. Its [stationary distribution](../../../../../../stationary-distribution.md) is

$$
\pi(\lambda)=\frac{(1-a_0-a_0b_1,\ a_0(1-a_0),\ a_0^2)}{1-a_0b_1}.
$$

The corresponding population limiting [expected value](../../../../../../expected-value.md) of the premium is $c\int_0^\infty[1-\alpha\pi_\alpha(\lambda)-\beta\pi_\beta(\lambda)]\nu e^{-\nu\lambda}\,d\lambda$. This gives the correct alternative when the intensity persists, and makes the extra assumption behind the requested marginal matrix explicit.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
