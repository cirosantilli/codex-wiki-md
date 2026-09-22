# Expected generation size in a Galton-Watson process

↑ **Parent:** [Galton-Watson process](galton-watson-process-split.md)

For a [Galton-Watson process](galton-watson-process-split.md) starting with one ancestor and finite offspring [mean](expected-value-split.md) $\mu$, the [expected value](expected-value-split.md) of the generation size is $\mathbb E[Z_n]=\mu^n$. At $n=0$ it is one, including when $\mu=0$; zero offspring [mean](expected-value-split.md) forces every later generation to be empty. With $m$ initial ancestors, the [expected value](expected-value-split.md) is $m\mu^n$.

For $p_0=p_1=1/4$, $p_2=1/2$, the offspring [mean](expected-value-split.md) is $5/4$. The exact calculations used in the generation [probability mass function](probability-mass-function.md) figure under [Galton-Watson process](galton-watson-process-split.md) give:

| Generation $n$ | Possible sizes | Extinction by $n$: $q_n$ | [Expected value](expected-value-split.md) $\mathbb E[Z_n]$ |
| --- | --- | --- | --- |
| 0 | 1 | 0 | 1 |
| 1 | 0–2 | 0.2500000000 | 1.25 |
| 2 | 0–4 | 0.3437500000 | 1.5625 |
| 3 | 0–8 | 0.3950195313 | 1.953125 |
| 4 | 0–16 | 0.4267750978 | 2.44140625 |
| 5 | 0–32 | 0.4477622665 | 3.0517578125 |
| 6 | 0–64 | 0.4621860903 | 3.814697265625 |

Nearly half the families are already empty at generation six, yet the [expected value](expected-value-split.md) exceeds three. Since empty families contribute zero,

$$
\mathbb E[Z_n\mid Z_n>0]=\frac{\mu^n}{1-q_n}
$$

whenever $q_n<1$. At generation six this [conditional expectation](conditional-expectation.md) is about $7.092969$. Conditioning on being nonempty now differs from conditioning on eventual survival: some presently nonempty families will still die out. The eventual [branching extinction probability](extinction-probability-of-a-branching-process.md) is $1/2$, even as the unconditional [expected value](expected-value-split.md) grows without bound.

The [expected value](expected-value-split.md) is useful for computing average population counts and, in the subcritical case, the [expected value](expected-value-split.md) of the [total progeny of a branching process](total-progeny-of-a-branching-process.md). Its simple formula comes from one local calculation: [linearity of expectation](linearity-of-expectation.md) and the [independent and identically distributed](independent-and-identically-distributed-random-variables.md) offspring counts give

$$
\mathbb E[Z_{n+1}\mid Z_n]=\mu Z_n,\qquad \mathbb E[Z_{n+1}]=\mu\mathbb E[Z_n].
$$

The [tower property of conditional expectation](law-of-total-expectation.md) gives the second equality; starting from $\mathbb E[Z_0]=1$ gives the formula. It describes an average over the generation [probability distribution](probability-distribution-split.md), not deterministic growth of an individual family. [University of Münster branching-process notes, Section 1.3, Proposition 1.4](https://www.uni-muenster.de/Stochastik/lehre/WS1011/SpezielleStochastischeProzesse/Ch_1.pdf)

## ↑ Ancestors (5)

1. [Galton-Watson process](galton-watson-process-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Extinction probability of a branching process](extinction-probability-of-a-branching-process.md)
- [Galton-Watson process](galton-watson-process-split.md)
- [Offspring distribution of a branching process](offspring-distribution-of-a-branching-process.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ia/paper-1/4f/solution.md)
- [Total progeny of a branching process](total-progeny-of-a-branching-process.md)
