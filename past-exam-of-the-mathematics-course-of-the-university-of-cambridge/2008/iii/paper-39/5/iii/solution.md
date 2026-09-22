<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [diffusion coefficient](../../../../../../diffusion-coefficient.md) becomes $S\sigma(S)=\sqrt S$, so the stock is a [driftless square-root diffusion](../../../../../../driftless-square-root-diffusion.md), with zero taken as an absorbing boundary. Substitution of $V(t,S)=e^{A(t)S+B(t)}$ into the [pricing equation for a local volatility model](../../../../../../pricing-equation-for-a-local-volatility-model.md) gives

$$
A'(t)S+B'(t)+\tfrac12A(t)^2S=0.
$$

Equating the constant and linear terms and imposing the terminal payoff gives

$$
A'+\tfrac12A^2=0,\quad B'=0,\quad A(1)=1,\quad B(1)=0.
$$

Thus $1/A(t)=(1+t)/2$ and $B(t)=0$, and the price is

$$
\boxed{\xi_t=V(t,S_t)=\exp\left(\frac{2S_t}{1+t}\right),\qquad 0\leq t\leq1.}
$$

This is the [exponential claim in a driftless square-root model](../../../../../../exponential-claim-in-a-driftless-square-root-model.md). At the absorbing boundary its value is $1$, matching the payoff at zero.

The payoff in this part is unbounded, unlike the payoff assumed in part (i), so it is useful to verify that the proposed price is a finite [conditional expectation](../../../../../../conditional-expectation.md). For $h>0$, starting from stock value $s$, define

$$
F(v,x)=\exp\left(-\frac{ux}{1+u(h-v)/2}\right),\qquad 0\leq v\leq h,\quad u\geq0.
$$

Then $F_v+\tfrac12xF_{xx}=0$, $F(h,x)=e^{-ux}$, and $0\leq F\leq1$. By [Itô formula](../../../../../../ito-s-lemma.md), $F(v,S_v)$ is a bounded [local martingale](../../../../../../local-martingale.md), hence a true [martingale](../../../../../../martingale-split.md). It follows that

$$
\mathbb E_s[e^{-uS_h}]=\exp\left(-\frac{su}{1+uh/2}\right).
$$

This is also the [Laplace transform](../../../../../../laplace-transform.md) of a sum of $N$ independent variables with [exponential distribution](../../../../../../exponential-distribution.md) of rate $2/h$, where $N$ has [Poisson distribution](../../../../../../poisson-distribution.md) of mean $2s/h$ and is independent of the summands: its transform is $\exp[(2s/h)((2/h)/(2/h+u)-1)]$. Uniqueness of the [Laplace transform](../../../../../../laplace-transform.md) therefore gives the [compound Poisson transition law of a driftless square-root diffusion](../../../../../../compound-poisson-transition-law-of-a-driftless-square-root-diffusion.md). The [exponential distribution](../../../../../../exponential-distribution.md) jump has [exponential moment](../../../../../../exponential-moment.md) $\mathbb E[e^{Y}]=(2/h)/(2/h-1)$ whenever $h<2$. Summing over the [Poisson distribution](../../../../../../poisson-distribution.md) yields

$$
\mathbb E_s[e^{S_h}]=\exp\left[\frac{2s}{h}\left(\frac{2/h}{2/h-1}-1\right)\right]=\exp\left(\frac{s}{1-h/2}\right).
$$

For the remaining horizon $h=1-t\leq1$, this is finite and, by the [Markov property](../../../../../../markov-property.md), is precisely $\mathbb E_Q[e^{S_1}\mid\mathcal F_t]=e^{2S_t/(1+t)}$. Thus the displayed process is indeed the [risk-neutral pricing](../../../../../../risk-neutral-pricing.md) value and a true [martingale](../../../../../../martingale-split.md). The [replicating strategy](../../../../../../replicating-strategy.md) from part (ii) has $h^S_t=[2/(1+t)]V(t,S_t)$ and $h^B_t=[1-2S_t/(1+t)]V(t,S_t)/B_t$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
