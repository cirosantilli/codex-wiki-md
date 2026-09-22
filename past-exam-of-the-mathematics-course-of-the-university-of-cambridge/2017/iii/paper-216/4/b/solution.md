<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A counterexample can use an irreducible, aperiodic [reversible Markov chain](../../../../../../reversible-markov-chain.md), so failure is not caused by a pathological transition structure. Take two binary coordinates, enumerate the four states as $00,01,10,11$, and let $\pi$ be their [uniform distribution](../../../../../../continuous-uniform-distribution.md). Use the [Markov kernel](../../../../../../markov-kernel.md)

$$
K=\begin{pmatrix}
1/4&1/4&1/4&1/4\\
1/4&1/2&1/8&1/8\\
1/4&1/8&1/2&1/8\\
1/4&1/8&1/8&1/2
\end{pmatrix}.
$$

Its rows sum to one and it is symmetric, proving [detailed balance](../../../../../../detailed-balance.md) with $\pi$. Every entry is positive. Let the univariate parametric family be $\widetilde{\mathcal Q}=\{\operatorname{Bernoulli}(r):0\leq r\leq2/5\}$.

For a product initial [probability distribution](../../../../../../probability-distribution.md) with parameters $r_1,r_2$, additivity of the [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md) gives

$$
\operatorname{KL}(\nu\Vert\pi)=\sum_{i=1}^2
\{r_i\log(2r_i)+(1-r_i)\log(2(1-r_i))\}.
$$

Each summand has [derivative](../../../../../../derivative.md) $\log(r_i/(1-r_i))<0$ on $(0,2/5]$, so the unique optimum at $t=0$ has $r_1=r_2=2/5$. Thus

$$
q^{*0}=(9,6,6,4)/25,
\qquad Kq^{*0}=(25,26,26,23)/100.
$$

On the other hand the allowed initial [probability distribution](../../../../../../probability-distribution.md) $\delta_{00}$, obtained with $r_1=r_2=0$, is sent by one step to $\pi$. Its [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md) is zero, the smallest possible value. Consequently

$$
\boxed{q^{*1}=\pi\ne Kq^{*0}.}
$$

The transition reduces [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md) for each input, but may reduce it by different amounts for different inputs. It therefore need not preserve the ordering of competing initial [probability distributions](../../../../../../probability-distribution.md), which is exactly why [Markov chain variational inference](../../../../../../markov-chain-variational-inference.md) must optimize the initial parameters for its chosen number of steps.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
