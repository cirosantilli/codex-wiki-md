<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use one particle for each telephone line, including unused lines. Let $f$ be the number of free lines, $h$ the number of callers waiting for or being checked by an operator, and $a$ the number using automated service. Then $f+h+a=N$. These are the three colonies of a [closed migration process](../../../../../closed-migration-process.md), with directed cycle $f\to h\to a\to f$ and departure rates

$$
\phi_f(f)=\nu\mathbf1_{\{f>0\}},\qquad
\phi_h(h)=\lambda\mathbf1_{\{h>0\}},\qquad
\phi_a(a)=\mu a.
$$

Rejected attempted calls leave the state unchanged. They must not be represented as extra customers in the waiting stage.

Equivalently the state is $(h,a)$ with $h+a\leq N$. Its transitions are

$$
(h,a)\to(h+1,a)\text{ at rate }\nu\quad(h+a<N),
$$



$$
(h,a)\to(h-1,a+1)\text{ at rate }\lambda\quad(h>0),\qquad
(h,a)\to(h,a-1)\text{ at rate }\mu a.
$$

The directed cycle has equal traffic weights; choosing each weight to be $\nu$ gives the unnormalized [product-form stationary distribution of a closed migration process](../../../../../product-form-stationary-distribution-of-a-closed-migration-process.md)

$$
w(h,a)=\left(\frac\nu\lambda\right)^h
\frac{(\nu/\mu)^a}{a!}.
$$

We can verify [global balance for a continuous-time Markov chain](../../../../../global-balance-for-a-continuous-time-markov-chain.md) directly. Weighted incoming transitions from $(h-1,a)$, $(h+1,a-1)$ and $(h,a+1)$ contribute, respectively,

$$
w(h,a)\lambda\mathbf1_{\{h>0\}},\qquad
w(h,a)\mu a,\qquad
w(h,a)\nu\mathbf1_{\{h+a<N\}}.
$$

Their sum equals the weight times the outgoing rate. This proves [stationarity](../../../../../stationary-process.md) after normalization, without falsely asserting reversibility of the directed migration cycle.

For $n=h+a$ occupied lines, summing over the automated population gives

$$
\sum_{a=0}^n w(n-a,a)
=\left(\frac\nu\lambda\right)^n
\sum_{a=0}^n\left(\frac\lambda\mu\right)^a\frac1{a!}=H(n).
$$

The [normalizing constant](../../../../../normalizing-constant.md) is $G_N=\sum_{n=0}^NH(n)$. The attempted calls form an independent [Poisson process](../../../../../poisson-process.md), so [Poisson arrivals see time averages](../../../../../poisson-arrivals-see-time-averages.md): the rate of attempted arrivals seeing a full state is $\nu$ times its stationary probability, and division by the total attempted-arrival rate gives the loss proportion. Consequently

$$
\boxed{P_{\mathrm{loss}}=\frac{H(N)}{\sum_{n=0}^NH(n)}.}
$$

The numerator is essential; the PDF contains it even though the converted TeX loses it.

With two independent operators, the total check-completion rate is $\lambda\min(h,2)$. In particular it is only $\lambda$ when one caller is present. Define

$$
D_2(h)=\prod_{j=1}^h\min(j,2)
=\begin{cases}1,&h=0,\\2^{h-1},&h\geq1.\end{cases}
$$

The human-stage weight becomes $(\nu/\lambda)^h/D_2(h)$, while the free and automated weights are unchanged. The same global-balance calculation applies using these departure rates. Thus

$$
H_2(n)=\sum_{a=0}^n
\frac{(\nu/\lambda)^{n-a}(\nu/\mu)^a}{D_2(n-a)a!},
\qquad
\boxed{P_{\mathrm{loss}}^{(2)}=\frac{H_2(N)}{\sum_{n=0}^NH_2(n)}.}
$$

This is the [blocking probability in a finite-line sequential-service network](../../../../../blocking-probability-in-a-finite-line-sequential-service-network.md) with two operators. It remains valid for $N=0$, when every attempted call is lost; for $N=1$ it coincides with the single-operator answer.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
