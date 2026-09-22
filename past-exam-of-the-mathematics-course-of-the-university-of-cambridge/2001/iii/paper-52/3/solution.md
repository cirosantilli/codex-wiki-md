<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [microparasite](../../../../../microparasite.md) typically multiplies within an infected [host](../../../../../host-biology.md) on a much shorter time scale than between-host transmission. A useful first model classifies [hosts](../../../../../host-biology.md) by infection status. A [macroparasite](../../../../../macroparasite.md), such as an adult parasitic worm, instead requires a count of [parasites](../../../../../parasite.md) per [host](../../../../../host-biology.md): two infected [hosts](../../../../../host-biology.md) can carry very different [within-host parasite burdens](../../../../../within-host-parasite-burden.md). These are modelling distinctions rather than a rule determined only by an organism's physical size.

For a [microparasite](../../../../../microparasite.md) with no lasting [immunity](../../../../../immunity-medical.md), a homogeneous [SIS model](../../../../../sis-model.md) is

$$
\dot I=\beta\frac{SI}{N}-\gamma I,
\qquad S+I=N.
$$

The [basic reproduction number](../../../../../basic-reproduction-number.md) is $\beta/\gamma$, and the [prevalence](../../../../../prevalence.md) $I/N$ describes the infected-host fraction. A [SIR model](../../../../../sir-model.md) adds an immune class, and a [SEIR model](../../../../../seir-model.md) adds a latent class. Contact structure, age, susceptibility, [recovery rate](../../../../../recovery-rate.md) and infectiousness can require several such classes. Then a [next-generation matrix](../../../../../next-generation-matrix.md) or operator, rather than a single averaged contact rate, sets the invasion threshold. [Stochastic epidemic models](../../../../../stochastic-epidemic-model.md) are relevant to early extinction and finite populations; network or spatial models represent nonuniform contact opportunities.

For a simple [macroparasite burden model](../../../../../macroparasite-burden-model.md), let $p_j$ be the fraction of [hosts](../../../../../host-biology.md) carrying $j$ adult worms. Assume acquisitions at rate $\lambda=\beta L$, independent adult-worm losses at rate $\mu j$, and a number $L$ of infective stages in a well-mixed environmental reservoir. The [immigration-death worm-burden model](../../../../../immigration-death-worm-burden-model.md) has

$$
\dot p_j=\lambda p_{j-1}+\mu(j+1)p_{j+1}-(\lambda+\mu j)p_j,
\qquad p_{-1}=0.
$$

This [birth-death process](../../../../../birth-death-process.md) needs the burden distribution or its [probability generating function](../../../../../probability-generating-function.md), not just an infected/not-infected partition. Its [mean](../../../../../expected-value.md) $m=\sum_jjp_j$ satisfies $\dot m=\beta L-\mu m$. With [host](../../../../../host-biology.md) number $N$ fixed and each adult producing infective stages at rate $\sigma$, one possible environmental closure is

$$
\dot L=\sigma Nm-(d_L+\beta N)L.
$$

For this asexual, unsaturated transmission approximation, one worm's [basic reproduction number](../../../../../basic-reproduction-number.md) is $(\sigma/\mu)\,\beta N/(d_L+\beta N)$. Growth above the invasion threshold requires additional density regulation if a finite endemic burden is sought. Sex-dependent mating would change this closure.

With constant external exposure $\lambda$, the [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) burden follows a [Poisson distribution](../../../../../poisson-distribution.md) with [mean](../../../../../expected-value.md) $m=\lambda/\mu$, giving infected-host [prevalence](../../../../../prevalence.md) $1-e^{-m}$. If exposure rates vary across [hosts](../../../../../host-biology.md) as a [gamma distribution](../../../../../gamma-distribution.md), the [Poisson-gamma mixture](../../../../../poisson-gamma-mixture.md) gives a [negative binomial distribution](../../../../../negative-binomial-distribution.md) with [mean](../../../../../expected-value.md) $m$ and aggregation parameter $k$:

$$
\operatorname{Var}(j)=m+\frac{m^2}{k},
\qquad \Pr(j>0)=1-\left(1+\frac{m}{k}\right)^{-k}.
$$

The same [mean](../../../../../expected-value.md) burden can therefore coexist with very different [prevalence](../../../../../prevalence.md) and highly infected subgroups. [Aggregation of macroparasite burdens](../../../../../aggregation-of-macroparasite-burdens.md) affects treatment coverage, burden-dependent [host](../../../../../host-biology.md) mortality, [immunity](../../../../../immunity-medical.md) and [parasite](../../../../../parasite.md) fecundity. For sexually reproducing worms, [hosts](../../../../../host-biology.md) need both sexes for fertile output; a [mean](../../../../../expected-value.md) alone may not determine it. With independent equally likely sexes and Poisson burden, the [probability](../../../../../probability.md) of both sexes is $(1-e^{-m/2})^2$, illustrating [mating-limited macroparasite transmission](../../../../../mating-limited-macroparasite-transmission.md) and its low-burden bottleneck.

Both [microparasite](../../../../../microparasite.md) and [macroparasite](../../../../../macroparasite.md) models need heterogeneous exposure and [host](../../../../../host-biology.md) responses. The special extra difficulty for [macroparasites](../../../../../macroparasite.md) is translating a distributed worm burden, and possibly worm sex or developmental stage, into transmission and [host](../../../../../host-biology.md) harm. Conversely, complicated within-host [microparasite](../../../../../microparasite.md) processes can also require more than a binary [host](../../../../../host-biology.md) state when the simple fast-within-host approximation fails.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
