# Offspring distribution of a branching process

↑ **Parent:** [Galton-Watson process](galton-watson-process.md)

The offspring [probability distribution](probability-distribution.md) of a [Galton-Watson process](galton-watson-process.md) is the law of one individual's number of children: $p_k=\mathbb P(\xi=k)$ for $k\geq0$, with $p_k\geq0$ and $\sum_{k\geq0}p_k=1$. Its [probability generating function](probability-generating-function.md) and, when finite, its [expected value](expected-value.md) are

$$
F(s)=\mathbb E[s^\xi]=\sum_{k\geq0}p_ks^k,\quad 0\leq s\leq1,\qquad \mu=\mathbb E[\xi]=\sum_{k\geq0}kp_k=F'(1-).
$$

Use $0^0=1$ when evaluating the [probability generating function](probability-generating-function.md) at zero: $F(0)=p_0$ and $F(1)=1$.

For $p_0=p_1=1/4$ and $p_2=1/2$, $F(s)=1/4+s/4+s^2/2$, $\mu=5/4$, and the offspring [variance](variance-split.md) is $11/16$: $\mathbb E[\xi^2]=9/4$ and $\operatorname{Var}(\xi)=9/4-(5/4)^2$. The generation [probability mass functions](probability-mass-function.md) pictured under [Galton-Watson process](galton-watson-process.md) come from repeatedly composing this [probability generating function](probability-generating-function.md). They describe the whole generation, whereas $(p_k)$ describes one individual's reproduction. [University of Münster branching-process notes, Section 1.3, Proposition 1.4](https://www.uni-muenster.de/Stochastik/lehre/WS1011/SpezielleStochastischeProzesse/Ch_1.pdf)

The whole [offspring distribution](offspring-distribution-of-a-branching-process.md) matters for extinction. Another law, $p_0=3/8$ and $p_2=5/8$, has the same offspring [mean](expected-value.md) $5/4$ but [branching extinction probability](extinction-probability-of-a-branching-process.md) $3/5$, since $3/8+5s^2/8=s$ has [roots of a polynomial](root-of-a-polynomial.md) $3/5$ and $1$. Consequently the two laws have the same [expected generation size in a Galton-Watson process](expected-generation-size-in-a-galton-watson-process.md) at each generation but different survival chances. A [binomial branching process](binomial-branching-process.md) and a [Poisson branching process](poisson-branching-process.md) likewise specify different [offspring distributions](offspring-distribution-of-a-branching-process.md); a common [mean](expected-value.md) does not make their [probability generating functions](probability-generating-function.md) identical.

**Table of contents**

- [Fractional-power offspring generating function](fractional-power-offspring-generating-function.md)

## ↑ Ancestors (5)

1. [Galton-Watson process](galton-watson-process.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
