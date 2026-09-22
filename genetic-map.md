# Genetic map

↑ **Parent:** [Genetic linkage](genetic-linkage.md)

A genetic map turns observations of inherited [haplotypes](haplotype.md) into an ordered account of [genetic loci](genetic-locus.md) along a [chromosome](chromosome.md). Its distances describe [genetic recombination](genetic-recombination.md), which makes the map useful for locating a [genetic locus](genetic-locus.md) relative to known [genetic markers](genetic-marker.md). A [genetic map](genetic-map.md) measures inheritance separation; separation measured in [base pairs](base-pair.md) describes positions along [DNA](deoxyribonucleic-acid.md). [Recombination hotspots](recombination-hotspot.md) help explain why equal numbers of [base pairs](base-pair.md) need not give equal [genetic map](genetic-map.md) distances. See [T. A. Brown, Genomes, 2nd edition (2002), chapter 5: Mapping Genomes](https://www.ncbi.nlm.nih.gov/books/NBK21116/).

Write $d$ for the [expected value](expected-value-split.md) of the number of [chromosomal crossovers](chromosomal-crossover.md) encountered along one transmitted [chromatid](chromatid.md) between the chosen [genetic loci](genetic-locus.md), measured in [morgans](morgan-unit.md); $100d$ is the distance in [centimorgans](centimorgan.md). This counts exchanges along that transmitted [chromatid](chromatid.md), rather than all exchanges in the four-[chromatid](chromatid.md) meiotic bundle. For a short interval with very few multiple exchanges, the [recombination fraction](recombination-fraction.md) satisfies $r\approx d$: about $1\%$ recombinant [gametes](gamete.md) then corresponds to about one [centimorgan](centimorgan.md).

For a longer interval, hidden even numbers of [chromosomal crossovers](chromosomal-crossover.md) make that approximation inaccurate. Under the [Haldane mapping function](haldane-mapping-function.md), $d=0.2$ [morgans](morgan-unit.md) gives $r\approx0.164840$; conversely $r=0.2$ gives $d\approx0.255413$ [morgans](morgan-unit.md), or $25.5413$ [centimorgans](centimorgan.md). Applying the inverse formula to an already specified [genetic map](genetic-map.md) distance would confuse a count with a [probability](probability.md).

[Genetic map](genetic-map.md) distances add along ordered adjacent intervals because the total exchange count is the sum of its interval counts. For [independent random variables](independent-random-variables.md) describing counts in disjoint intervals of the [Haldane mapping function](haldane-mapping-function.md) model, the endpoint [recombination fraction](recombination-fraction.md) instead obeys

$$
r_{12}=r_1(1-r_2)+(1-r_1)r_2=r_1+r_2-2r_1r_2.
$$

Exactly one interval must change parental origin. Thus $r_1=r_2=0.2$ gives $r_{12}=0.32$, although the two [genetic map](genetic-map.md) distances add to approximately $0.510826$ [morgans](morgan-unit.md). The simple composition formula requires the stated [independence](independent-random-variables.md); [crossover interference](crossover-interference.md) can invalidate it.

**Table of contents**

- [Haldane mapping function](haldane-mapping-function.md)
- [Morgan (unit)](morgan-unit.md)
  - [Centimorgan](centimorgan.md)

## ↑ Ancestors (4)

1. [Genetic linkage](genetic-linkage.md)
2. [Genetics](genetics-split.md)
3. [Biology](biology-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Centimorgan](centimorgan.md)
- [Genetic map](genetic-map.md)
- [Genetic recombination](genetic-recombination.md)
- [Haldane mapping function](haldane-mapping-function.md)
- [Morgan (unit)](morgan-unit.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-57/6/a/solution.md)
- [Recombination fraction](recombination-fraction.md)
