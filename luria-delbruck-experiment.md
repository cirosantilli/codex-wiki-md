<h1 id="luria-delbruck-experiment">Luria-Delbrück experiment</h1>

↑ **Parent:** [Mutation](mutation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Luria–Delbrück_experiment)

In 1943, [Salvador Luria](salvador-luria.md) and [Max Delbrück](max-delbruck.md) grew separate [Escherichia coli](escherichia-coli.md) B [cell cultures](cell-culture.md) from small equal inocula, without the challenging [bacteriophage](bacteriophage.md). They used nutrient broth or an asparagine–glucose [cell culture medium](cell-culture-medium.md). On nutrient agar plates, they first spread excess [bacteriophage](bacteriophage.md) and then the bacterial sample centrally, leaving an outer margin. After incubation, resistant [biological colonies](colony-biology.md) provided the readout; counts were usually made at 24 and 48 hours. Their control plated repeated samples from one shared culture. Independently grown cultures varied much more than this sampling comparison. That contrast supported resistant lineages arising before challenge: early [mutations](mutation.md) could produce many resistant descendants before [natural selection](natural-selection.md) revealed them.[pp. 501–504, Material and Methods; Experimental, plating reliability, Table 1 and independent cultures, Table 2](mutations-of-bacteria-from-virus-sensitivity-to-virus-resistance-by-salvador-luria-and-max-delbruck.md)

This was evidence about the timing of heritable resistance, not [DNA sequencing](dna-sequencing.md) of the responsible [genes](gene.md). It does not establish uniform [mutation rates](mutation-rate.md) or exclude environmentally induced [mutations](mutation.md); the paper itself discusses physiological dependence and delayed expression.[pp. 505–507, discussion of excess variation, physiological state, delayed resistance and genetic relatedness](mutations-of-bacteria-from-virus-sensitivity-to-virus-resistance-by-salvador-luria-and-max-delbruck.md)

Now construct a deliberately small [mathematical model](mathematical-model.md) of the timing effect. Start with one sensitive [biological cell](biological-cell-split.md) at generation $g=0$. Every [biological cell](biological-cell-split.md) divides into two in each of five synchronous rounds, with no death or growth difference. There are $N_g=2^g$ [biological cells](biological-cell-split.md) immediately after round $g$, ending with $N_5=32$. In each scenario, exactly one newly formed daughter changes to resistance immediately after round $g$; its descendants inherit resistance without reversion or further [mutations](mutation.md). Resistance is expressed immediately, and the final challenge allows every resistant [biological cell](biological-cell-split.md), and no sensitive one, to form one separate [biological colony](colony-biology.md).

<a id="image-hypothetical-five-doubling-cell-lineages-one-early-mutation-makes-a-larger-resistant-family"></a>
![](mutation-timing-clonal-jackpot.png)

**[Figure 4](#image-hypothetical-five-doubling-cell-lineages-one-early-mutation-makes-a-larger-resistant-family). Hypothetical five-doubling cell lineages: one early mutation makes a larger resistant family**. Two constructed scenarios with 32 final [biological cells](biological-cell-split.md) each. An event after round 1 leaves four doublings and produces 16 resistant descendants; an event after round 4 leaves one doubling and produces 2. Orange marks the affected [cell lineage](cell-lineage.md). These are stipulated lineage trees, not the 1943 experiment's [biological colony](colony-biology.md) counts or a fitted [mutation rate](mutation-rate.md).

The descendant count obeys

$$
R_g=2^{5-g},\qquad g\in\{1,2,3,4,5\}.
$$

At the moment of the event there is one resistant [biological cell](biological-cell-split.md); each remaining round doubles its descendants. This proves the formula by repeated multiplication, with terminal case $R_5=1$. An event after round 1 gives $R_1=16$ resistant and 16 sensitive [biological cells](biological-cell-split.md); an event after round 4 gives $R_4=2$ resistant and 30 sensitive [biological cells](biological-cell-split.md). Both scenarios contain one [mutation](mutation.md) event. A culture with no event gives zero resistant [biological colonies](colony-biology.md) under these assumptions. The difference is family size, rather than the number of events.

For comparison, suppose each of the 32 final sensitive [biological cells](biological-cell-split.md) independently acquires resistance only on challenge, with [probability](probability.md) $p=1/16$ and no subsequent multiplication before counting. Then the resistant count has a [binomial distribution](binomial-distribution.md), with [expected value](expected-value-split.md) $32p=2$ and [variance](variance-split.md) $32p(1-p)=15/8$. This alternative [mathematical model](mathematical-model.md) has no pre-challenge resistant family to amplify. Its independent trials are an assumption of the comparison, not a consequence of using physically distinct [biological cells](biological-cell-split.md). The clonal scenarios explain how a jackpot can occur; they do not assign [probabilities](probability.md) to the event times or estimate a real [mutation rate](mutation-rate.md).

// Target: biology.bigb

## ↑ Ancestors (4)

1. [Mutation](mutation.md)
2. [Genetics](genetics-split.md)
3. [Biology](biology-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Bacteriophage](bacteriophage.md)
- [Lederberg replica plating experiment](lederberg-replica-plating-experiment.md)
- [Mutation](mutation.md)
