<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $a=p(x)q(x,y)$ and $b=p(y)q(y,x)$. For $a+b>0$, the off-diagonal [probability](../../../../../probability.md) flux of the proposed rule is

$$
p(x)q(x,y)\beta(x,y)=a\frac{b}{a+b}=\frac{ab}{a+b}=b\frac{a}{a+b}=p(y)q(y,x)\beta(y,x).
$$

If $a=b=0$, define both acceptance [probabilities](../../../../../probability.md) to be zero; both fluxes are zero. The diagonal [detailed balance equations](../../../../../detailed-balance.md) hold automatically, including the [probability](../../../../../probability.md) of rejected proposals. Summing the [detailed balance equations](../../../../../detailed-balance.md) over $x$ gives [stationarity](../../../../../stationary-process.md):

$$
\sum_xp(x)P(x,y)=\sum_xp(y)P(y,x)=p(y).
$$

**The alternative rule therefore preserves $p$.** The unknown [normalizing constant](../../../../../normalizing-constant.md) cancels after replacing $p$ by $r$. This [Barker acceptance probability](../../../../../barker-acceptance-probability.md) is no larger than the [Metropolis–Hastings acceptance probability](../../../../../metropolis-hastings-acceptance-probability.md) for the same proposed move: if $t=b/a>0$, then $t/(1+t)\leq\min(1,t)$. Preservation of $p$ still requires separate [Markov chain irreducibility](../../../../../irreducible-markov-chain.md) and convergence checks before it guarantees useful sampling.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Bayesian statistical probabilistic programming](../../../bayesian-statistical-probabilistic-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
