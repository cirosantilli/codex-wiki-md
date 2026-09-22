# Paper 45

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper45.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper45.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
  - [g](#3/g)
    - [Solution](#3/g/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
  - [f](#4/f)
    - [Solution](#4/f/solution)
  - [g](#4/g)
    - [Solution](#4/g/solution)

## 1

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Treat $G_i$ as the entire [phase-known genotype](../../../biology.md#phase-known-genotype) of individual $i$ at the [genetic loci](../../../biology.md#genetic-locus) being studied, and let $\overline F$ denote the nonfounders. Assume unrelated [pedigree founders](../../../biology.md#founder-in-a-pedigree) have independent [genotype](../../../biology.md#genotype) priors, each nonfounder's [genotype](../../../biology.md#genotype) depends only on its parents' [genotypes](../../../biology.md#genotype), and the observed [phenotypes](../../../biology.md#phenotype) are conditionally independent given the [genotypes](../../../biology.md#genotype). These are the standard assumptions behind the [pedigree likelihood](../../../biology.md#pedigree-likelihood); shared environmental effects or related [pedigree founders](../../../biology.md#founder-in-a-pedigree) would require additional factors.

The directed ancestry graph is acyclic, even when there is [inbreeding](../../../biology.md#inbreeding). Order individuals with parents preceding offspring and apply the [chain rule for probabilities](../../../probability-theory.md#chain-rule-for-probabilities). The parental [conditional independence](../../../random-variable.md#conditional-independence) assumption gives

$$
P(G_1,\ldots,G_n)=\prod_{i\in F}P(G_i)\prod_{i\in\overline F}P(G_i\mid G_{m(i)},G_{f(i)}).
$$

Conditional [phenotype](../../../biology.md#phenotype) [independence](../../../random-variable.md#independent-random-variables) gives $P(X_1,\ldots,X_n\mid G_1,\ldots,G_n)=\prod_iP(X_i\mid G_i)$. Multiplying these two expressions and summing over every possible latent [genotype](../../../biology.md#genotype) configuration proves

$$
\boxed{P(X_1,\ldots,X_n)=\sum_{G_1}\cdots\sum_{G_n}
\prod_iP(X_i\mid G_i)\prod_{i\in F}P(G_i)
\prod_{i\in\overline F}P(G_i\mid G_{m(i)},G_{f(i)}).}
$$

This is the [law of total probability](../../../probability-theory.md#law-of-total-probability), not a claim that relatives have independent unconditional [genotypes](../../../biology.md#genotype).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

For a binary disease [phenotype](../../../biology.md#phenotype), put $p_i(g)=P(X_i=\text{affected}\mid G_i=g)$. The [penetrance](../../../biology.md#penetrance) function depends on the inheritance model, the disease [alleles](../../../biology.md#allele) and [genotype](../../../biology.md#genotype), and potentially age, sex, environment and other genetic modifiers. Phenocopies allow disease without the putative disease [genotype](../../../biology.md#genotype), while incomplete [penetrance](../../../biology.md#penetrance) allows a [genetic carrier](../../../biology.md#genetic-carrier) of that [genotype](../../../biology.md#genotype) to remain unaffected. Thus the [phenotype](../../../biology.md#phenotype) factor is $p_i(g)$ for an affected individual and $1-p_i(g)$ for an unaffected one.

Under a fully penetrant model with no phenocopies the [genotype](../../../biology.md#genotype) determines disease status, so **the factor is 1 for a compatible [genotype](../../../biology.md#genotype) and 0 for an incompatible [genotype](../../../biology.md#genotype)**. For example, in fully penetrant [recessive inheritance](../../../biology.md#recessive-inheritance), $aa$ is affected and $AA,Aa$ are unaffected. Missing [phenotype](../../../biology.md#phenotype) observations contribute the constant factor 1 rather than excluding [genotypes](../../../biology.md#genotype).

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Without [genotyping error](../../../biology.md#genotyping-error), the observed [genetic marker](../../../biology.md#genetic-marker) [genotype](../../../biology.md#genotype) is a deterministic function $u(g)$ of the underlying [phase-known genotype](../../../biology.md#phase-known-genotype). In particular $u$ can forget chromosome phase and parental origin. Therefore

$$
\boxed{P(X_i=x\mid G_i=g)=\mathbf1_{\{u(g)=x\}}.}
$$

Several different phased [haplotype](../../../biology.md#haplotype) pairs can receive factor 1 when the observed multilocus [genotype](../../../biology.md#genotype) is unphased. With laboratory error, missing [alleles](../../../biology.md#allele) or uncertain calls, replace the indicator by an error or observation model. A wholly unobserved [genetic marker](../../../biology.md#genetic-marker) contributes factor 1. Thus a 0-or-1 factor reflects perfect observation of a deterministic [genetic marker](../../../biology.md#genetic-marker) state, not a general property of every genetic measurement.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [pedigree founder](../../../biology.md#founder-in-a-pedigree) factor $P(G_i)$ depends on population [allele](../../../biology.md#allele) and [haplotype](../../../biology.md#haplotype) frequencies, ancestry, mating assumptions and any population [linkage disequilibrium](../../../biology.md#linkage-disequilibrium). At one autosomal [genetic locus](../../../biology.md#genetic-locus), [Hardy-Weinberg equilibrium](../../../biology.md#hardy-weinberg-principle) with [allele](../../../biology.md#allele) frequencies $p,q$ gives [genotype](../../../biology.md#genotype) [probabilities](../../../probability-theory.md#probability) $p^2,2pq,q^2$. For a specified ordered pair of independent [pedigree founder](../../../biology.md#founder-in-a-pedigree) [haplotypes](../../../biology.md#haplotype) $h_1,h_2$, the [probability](../../../probability-theory.md#probability) is $p_{h_1}p_{h_2}$; an unordered distinct pair has twice that [probability](../../../probability-theory.md#probability). [Pedigree founders](../../../biology.md#founder-in-a-pedigree) assumed to be related require a joint prior rather than a product of unrelated-founder factors.

The nonfounder factor depends on the parental [genotypes](../../../biology.md#genotype) and phases, [Mendelian segregation](../../../biology.md#mendelian-segregation), and the [recombination fractions](../../../biology.md#recombination-fraction) between [genetic loci](../../../biology.md#genetic-locus). In a two-locus [heterozygote](../../../biology.md#heterozygote) of known phase, the two parental [haplotypes](../../../biology.md#haplotype) have transmission [probabilities](../../../probability-theory.md#probability) $(1-\theta)/2$ each, and the two recombinant [haplotypes](../../../biology.md#haplotype) $\theta/2$ each. Multiply the maternal and paternal gamete [probabilities](../../../probability-theory.md#probability) and sum any gamete combinations producing the child's [genotype](../../../biology.md#genotype). Sex-specific [genetic recombination](../../../biology.md#genetic-recombination), mutation or segregation distortion can be incorporated by changing these gamete [probabilities](../../../probability-theory.md#probability). At one ordinary autosomal [genetic locus](../../../biology.md#genetic-locus), each parental copy is transmitted with [probability](../../../probability-theory.md#probability) $1/2$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Call the parent [genotype](../../../biology.md#genotype) $g$ and child [genotype](../../../biology.md#genotype) $h$, each in $\{0,1\}$. Define

$$
a_g=P(X_p\mid G_p=g),\quad p_g=P(G_p=g),\quad
b_h=P(X_c\mid G_c=h),\quad t_{h\mid g}=P(G_c=h\mid G_p=g).
$$

There is one [pedigree founder](../../../biology.md#founder-in-a-pedigree) and one nonfounder, so

$$
\boxed{L=\sum_{g=0}^1\sum_{h=0}^1 a_gp_gb_ht_{h\mid g}.}
$$

Explicitly this is $a_0p_0b_0t_{0\mid0}+a_0p_0b_1t_{1\mid0}+a_1p_1b_0t_{0\mid1}+a_1p_1b_1t_{1\mid1}$. The genotype-transmission model can be arbitrary for the single-parent species; no two-parent Mendelian assumption is being introduced.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

In the unrearranged [likelihood](../../../statistical-modelling.md#likelihood-function) there are four summands. Each is a product of four supplied [probabilities](../../../probability-theory.md#probability) and takes three multiplications. Summing the four results takes three additions. Thus

$$
\boxed{12\text{ multiplications},\qquad3\text{ additions}.}
$$

This count concerns direct evaluation without reusing repeated factors; zero-or-one [phenotype](../../../biology.md#phenotype) values could of course allow extra special-case savings.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

The [Elston-Stewart algorithm](../../../biology.md#elston-stewart-algorithm) first sums over the child:

$$
L=\sum_{g=0}^1a_gp_g\left(b_0t_{0\mid g}+b_1t_{1\mid g}\right).
$$

For each of the two parent states, the inner message requires two multiplications and one addition, totaling four multiplications and two additions. Multiplying each message by its two parent factors takes two further multiplications per parent state, totaling four. The final sum uses one addition. Therefore

$$
\boxed{8\text{ multiplications},\qquad3\text{ additions}.}
$$

Moving the sum inward saves four multiplications because the factors independent of the child [genotype](../../../biology.md#genotype) are evaluated only once per parent state.

## 2

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

[Genetic linkage](../../../biology.md#genetic-linkage) analysis follows co-segregation of [genetic marker](../../../biology.md#genetic-marker) and disease [alleles](../../../biology.md#allele) within [pedigrees](../../../biology.md#pedigree). It estimates or tests a [recombination fraction](../../../biology.md#recombination-fraction), with [independent assortment](../../../biology.md#independent-assortment) at $\theta=1/2$ as the ordinary null. It can locate a disease [genetic locus](../../../biology.md#genetic-locus) even when different families have different [genetic marker](../../../biology.md#genetic-marker) [alleles](../../../biology.md#allele) on their disease chromosomes.

[Genetic association](../../../biology.md#genetic-association) analysis tests whether [allele](../../../biology.md#allele) or [genotype](../../../biology.md#genotype) frequencies differ with disease status. It can compare unrelated cases and controls, or compare transmitted and untransmitted parental [alleles](../../../biology.md#allele). A noncausal [genetic marker](../../../biology.md#genetic-marker) can be associated through population [linkage disequilibrium](../../../biology.md#linkage-disequilibrium) with a causal [genetic locus](../../../biology.md#genetic-locus). Association therefore concerns population-frequency relationships, whereas linkage concerns inheritance; [population stratification](../../../biology.md#population-stratification) can confound the former without producing genuine within-family linkage.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Only [heterozygous](../../../biology.md#heterozygosity) parents contribute an alternative-allele transmission contrast to the [transmission disequilibrium test](../../../biology.md#transmission-disequilibrium-test). Both parents are [homozygous](../../../biology.md#homozygosity) in rows 1, 13, 14 and 15, so **rows 1, 13, 14 and 15 are uninformative**. Their counts total 15 families. Every other row has at least one [heterozygous](../../../biology.md#heterozygosity) parent. When both parents are [heterozygous](../../../biology.md#heterozygosity) and the child is [heterozygous](../../../biology.md#heterozygosity), there is one transmission of each [allele](../../../biology.md#allele), regardless of the unresolved parent-specific phase; these transmissions contribute to both discordant cells.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Write $b$ for transmission of [allele](../../../biology.md#allele) 1 with [allele](../../../biology.md#allele) 2 untransmitted, and $c$ for the reverse. The informative transmissions give $b=20$, $c=30$. Under the fair-transmission null, conditional on $b+c=50$, $b$ is binomial with success [probability](../../../probability-theory.md#probability) $1/2$. Its standardized squared deviation is

$$
\boxed{\mathrm{TDT}=\frac{(b-c)^2}{b+c}=\frac{(20-30)^2}{50}=2.}
$$

The reference distribution is asymptotically chi-squared with one degree of freedom, giving a two-sided $p$-value about $0.157$. **[Allele](../../../biology.md#allele) 2 is overtransmitted and hence is the [allele](../../../biology.md#allele) more associated with disease in this sample**, although this result is not strong evidence against the null. The diagonal transmission cells contribute no discordant contrast.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Summing the transmission table by its rows and columns gives

$$
\begin{array}{c|cc}
&\text{transmitted}&\text{not transmitted}\\\hline
\text{allele 2}&59&49\\
\text{allele 1}&41&51
\end{array}
$$

Thus the marginal case-versus-pseudo-control [odds ratio](../../../statistical-modelling.md#odds-ratio) is

$$
\boxed{\widehat{\mathrm{OR}}=\frac{59/41}{49/51}=\frac{3009}{2009}\simeq1.498.}
$$

This is the requested approximate allelic effect. Keeping the parent-specific matching instead gives the discordant-pair [odds ratio](../../../statistical-modelling.md#odds-ratio) $c/b=30/20=1.5$, numerically close here. Neither calculation makes the within-family [allele](../../../biology.md#allele) observations independent population samples.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

For each family combine the two untransmitted parental [alleles](../../../biology.md#allele) into one [family pseudo-control genotype](../../../biology.md#family-pseudo-control-genotype). A [heterozygous](../../../biology.md#heterozygosity) child of two [heterozygous](../../../biology.md#heterozygosity) parents has a [heterozygous](../../../biology.md#heterozygosity) pseudo-control, whatever its parent-specific transmission phase. Combining the rows gives

$$
\boxed{(N_{11},N_{12},N_{22})=(13,25,12).}
$$

For example, pseudo-control [genotype](../../../biology.md#genotype) $1/1$ receives contributions $1,2,5,5$ from the relevant rows; [genotype](../../../biology.md#genotype) $2/2$ receives $3,1,2,6$, and the remaining 25 are [heterozygous](../../../biology.md#heterozygosity). These counts also give the untransmitted [allele](../../../biology.md#allele) totals 51 and 49.

The estimated [allele](../../../biology.md#allele) frequencies are $\widehat p_1=0.51$, $\widehat p_2=0.49$. The [Hardy-Weinberg equilibrium](../../../biology.md#hardy-weinberg-principle) expected [genotype](../../../biology.md#genotype) counts are

$$
50(\widehat p_1^2,2\widehat p_1\widehat p_2,\widehat p_2^2)=(13.005,24.990,12.005).
$$

They are almost identical to the observations, so **these pseudo-control counts conform extremely closely to [HWE](../../../biology.md#hardy-weinberg-principle) proportions**. The usual Pearson discrepancy is only about $8.0\times10^{-6}$. This numerical agreement is not a general guarantee of [HWE](../../../biology.md#hardy-weinberg-principle) for family pseudo-controls, whose construction involves mating structure and case [ascertainment in a genetic study](../../../biology.md#genetic-study-ascertainment).

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Family comparisons condition on the parental [genotypes](../../../biology.md#genotype), so cases are compared with the [alleles](../../../biology.md#allele) they could have inherited. This protects a transmission test from ordinary [population stratification](../../../biology.md#population-stratification), avoids having to recruit unrelated controls matched for ancestry, and can resolve [haplotypes](../../../biology.md#haplotype) and identify Mendelian inconsistencies. The same [pedigree](../../../biology.md#pedigree) may also provide linkage information.

The costs are recruiting and genotyping relatives, missing or unavailable parents, and fewer informative comparisons because [homozygous](../../../biology.md#homozygosity) parents contribute no transmission contrast. These problems are especially important for late-onset disease. Related cases or multiple siblings also require an analysis accounting for dependence, and [genotyping error](../../../biology.md#genotyping-error) or transmission distortion can mimic overtransmission. Population-based case/control studies are usually easier to assemble and can offer greater power per genotyped person, but need careful control of ancestry and other sources of confounding. Family sampling does not remove every form of [ascertainment in a genetic study](../../../biology.md#genetic-study-ascertainment) or observation bias.

## 3

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Fix one particular ancestral [allele](../../../biology.md#allele) copy $q$ among the four copies in the founding couple. The [pedigree founder](../../../biology.md#founder-in-a-pedigree) carrying it transmits it independently to each of the two generation-2 siblings with [probability](../../../probability-theory.md#probability) $1/2$. Therefore

$$
\boxed{P(q\text{ reaches both siblings})=(1/2)^2=1/4.}
$$

Here “one copy” means a specified copy, as required to follow “this ancestral copy” in the subsequent parts. If instead one asks whether the siblings share at least one of the four copies without specifying which, the [probability](../../../probability-theory.md#probability) is $1-(1/2)^2=3/4$: they fail to share either the paternal or maternal copy with [probability](../../../probability-theory.md#probability) $1/4$. These are different events.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Conditional on both generation-2 siblings carrying the specified copy $q$, each passes it to each of their three children with [probability](../../../probability-theory.md#probability) $1/2$. Their outside partners do not carry that ancestral copy. There are six independent [meioses](../../../biology.md#meiosis), one for each generation-3 individual forming the three cousin marriages. Consequently

$$
\boxed{P(\text{all six generation-3 partners carry }q\mid\text{both generation-2 siblings carry }q)=2^{-6}=1/64.}
$$

This calculation ignores [phenotype](../../../biology.md#phenotype) [ascertainment in a genetic study](../../../biology.md#genetic-study-ascertainment), as requested; conditioning on the later disease observations would force these transmissions rather than assign them their prior [probabilities](../../../probability-theory.md#probability).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Each relevant cousin marriage is a cross between two [genetic carriers](../../../biology.md#genetic-carrier) of $q$. A child receives two copies of $q$ with [probability](../../../probability-theory.md#probability) $(1/2)(1/2)=1/4$, and fails to receive two with [probability](../../../probability-theory.md#probability) $3/4$. Conditional on the parental [genotypes](../../../biology.md#genotype), distinct offspring transmissions are independent. There are eight specified double-copy children and eight specified remaining children, giving

$$
\boxed{P=(1/4)^8(3/4)^8=\frac{3^8}{4^{16}}.}
$$

There are no [binomial coefficients](../../../combinatorics.md#binomial-coefficient) because the subjects have been individually selected. If only the counts in the three sibships were specified, rather than their identities, the [probability](../../../probability-theory.md#probability) would instead be multiplied by $\binom11\binom74\binom83=1960$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $E_q$ be the event that all eight selected subjects carry two copies of the same specified ancestral copy $q$, and that no other generation-4 subject is [autozygous](../../../biology.md#autozygosity) at this [genetic locus](../../../biology.md#genetic-locus). The selected subjects occur in every sibship, so this event forces both generation-2 transmissions and all six relevant generation-3 transmissions. Applying the preceding conditional [probabilities](../../../probability-theory.md#probability),

$$
P(E_q)=\frac14\frac1{64}\left(\frac14\right)^8\left(\frac34\right)^8
=\frac{3^8}{2^{40}}.
$$

Once all six parents carry $q$, their other copies come from the two unrelated outside [pedigree founders](../../../biology.md#founder-in-a-pedigree), one on each side of the [pedigree](../../../biology.md#pedigree). A child not receiving two $q$ copies therefore cannot become [autozygous](../../../biology.md#autozygosity) for a different founding copy. This verifies the “only” condition, rather than merely excluding [homozygosity](../../../biology.md#homozygosity) for $q$.

For the event $E$ without specifying which of the original four copies is shared, the four alternatives $E_q$ are disjoint: a selected child cannot simultaneously have both its copies descended from two different ancestral copies. Hence

$$
\boxed{P(E)=4P(E_q)=\frac{3^8}{2^{38}}.}
$$

All selected individuals are then [autozygous](../../../biology.md#autozygosity) for the same copy and mutually 2-IBD. The distinction from the $3/4$ [probability](../../../probability-theory.md#probability) in the alternative interpretation of part (a) is precisely this disjointness.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Let $D$ denote the specified disease pattern. With one introduced disease-allele copy, no new mutations or phenocopies, and fully penetrant [recessive inheritance](../../../biology.md#recessive-inheritance), every affected subject must carry two descendants of that one copy. Since every sibship has an affected child, all the upstream [genetic carrier](../../../biology.md#genetic-carrier) transmissions described above are forced. Conversely, unaffected siblings cannot carry two disease copies. Thus $D$ implies the inheritance event $E$ at the causal [genetic locus](../../../biology.md#genetic-locus), and

$$
\boxed{P(E\mid D)=1.}
$$

The rarity of the unconditional pattern in part (d) does not make its [posterior probability](../../../statistical-inference.md#posterior-probability) small after observing the pattern that forces it. If the location of the one disease copy is initially uniform among the four founding copies, the [likelihood](../../../statistical-modelling.md#likelihood-function) of $D$ is the same for each, so its posterior location remains uniform; $P(E_q\mid D)=1/4$ for any named copy. If $q$ is already designated as the disease copy, its corresponding event has [posterior probability](../../../statistical-inference.md#posterior-probability) 1.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

Write $D$ for the disease observations and $M$ for the [genetic marker](../../../biology.md#genetic-marker) observations. The [LOD score](../../../biology.md#lod-score) for [complete linkage](../../../biology.md#complete-genetic-linkage) is

$$
\boxed{Z(0)=\log_{10}\frac{P(M\mid D,\theta=0)}{P(M\mid D,\theta=1/2)}.}
$$

The disease marginal cancels because the single-locus disease segregation law does not depend on the [genetic marker](../../../biology.md#genetic-marker)–disease [recombination fraction](../../../biology.md#recombination-fraction). The ten [genetic markers](../../../biology.md#genetic-marker) form one nonrecombining [haplotype](../../../biology.md#haplotype); they do not supply ten independent copies of the [pedigree](../../../biology.md#pedigree)'s segregation evidence.

There is a distinction between [identity by state](../../../biology.md#identity-by-state) and [identity by descent](../../../biology.md#identity-by-descent). The reported observation that affected subjects all have $h/h$ establishes the former. An exact [genetic marker](../../../biology.md#genetic-marker) [likelihood](../../../statistical-modelling.md#likelihood-function) requires [pedigree founder](../../../biology.md#founder-in-a-pedigree) [haplotype](../../../biology.md#haplotype) frequencies, or the actual [pedigree founder](../../../biology.md#founder-in-a-pedigree) [genotypes](../../../biology.md#genotype) if conditioning on them. Here is an explicit expression using independent [pedigree founder](../../../biology.md#founder-in-a-pedigree) [haplotypes](../../../biology.md#haplotype), with frequency $p$ for the observed [haplotype](../../../biology.md#haplotype) $h$, and linkage equilibrium between [pedigree founder](../../../biology.md#founder-in-a-pedigree) [genetic marker](../../../biology.md#genetic-marker) and disease states. There are eight [genetic marker](../../../biology.md#genetic-marker) copies in the four [pedigree founders](../../../biology.md#founder-in-a-pedigree): the original couple and the two generation-2 outside spouses. For [genetic marker](../../../biology.md#genetic-marker) inheritance configuration $v$, let $K(v)$ be the number of distinct [pedigree founder](../../../biology.md#founder-in-a-pedigree) copies ancestral to the sixteen chromosome copies in the eight selected subjects. Then

$$
R(p)=\sum_v P(v)p^{K(v)}=E[p^K]
$$

is the unlinked [probability](../../../probability-theory.md#probability) that all those copies have state $h$. At [complete linkage](../../../biology.md#complete-genetic-linkage) the affected subjects all inherit the disease [pedigree founder](../../../biology.md#founder-in-a-pedigree) copy twice, and the [probability](../../../probability-theory.md#probability) that this copy has [genetic marker](../../../biology.md#genetic-marker) state $h$ is $p$. Therefore

$$
\boxed{Z(0)=\log_{10}\frac{p}{R(p)}.}
$$

The denominator can be evaluated without an unspecified inheritance sum. Let $B_a=\binom2a p^a(1-p)^{2-a}$ for $a=0,1,2$. If parental [genetic marker](../../../biology.md#genetic-marker) [genotypes](../../../biology.md#genotype) contain $a,b$ copies of $h$, the child count distribution is

$$
Q_0(a,b)=(1-a/2)(1-b/2),\quad
Q_1(a,b)=(a/2)(1-b/2)+(1-a/2)(b/2),\quad
Q_2(a,b)=ab/4.
$$

For a generation-2 couple define

$$
F(a,b)=\prod_{r\in\{1,4,3\}}\left[\sum_{j=0}^2Q_j(a,b)(j/2)^r\right],\qquad
m_a=\sum_{b=0}^2B_bF(a,b).
$$

For a particular generation-3 parent with $j$ [genetic marker](../../../biology.md#genetic-marker) copies, the chance it transmits $h$ to all its $r$ selected offspring is $(j/2)^r$, which explains each factor. Conditional on the original founding couple, its two generation-2 siblings and their independent outside spouses give independent left and right contributions. Thus

$$
R(p)=\sum_{u,v=0}^2B_uB_v\left[\sum_{a=0}^2Q_a(u,v)m_a\right]^2.
$$

Expanding gives

$$
R(p)=\frac{p}{2^{22}}\left(1+388p+38942p^2+480421p^3+1398448p^4+1540264p^5+650576p^6+85264p^7\right).
$$

It satisfies $R(1)=1$, as it must for a monomorphic [haplotype](../../../biology.md#haplotype). This expression supplies a numerical LOD once $p$ is specified; the problem does not specify that frequency.

In the idealized limit where a matching rare [haplotype](../../../biology.md#haplotype) identifies one ancestral copy, the leading coefficient is particularly simple. Dropping restrictions on the eight unaffected subjects, the [probability](../../../probability-theory.md#probability) that all selected subjects are [autozygous](../../../biology.md#autozygosity) for one common copy is

$$
P(H)=4\cdot\frac14\cdot\frac1{64}\cdot\left(\frac14\right)^8=2^{-22}.
$$

Accordingly $R(p)/p\to2^{-22}$ as $p\to0$, and the affected-only [IBD](../../../biology.md#identity-by-descent) calculation gives $Z(0)=22\log_{10}2\simeq6.623$.

If the [genetic marker](../../../biology.md#genetic-marker) observations additionally establish the exact pattern $E$ of part (d), including that the eight unaffected subjects are not [autozygous](../../../biology.md#autozygosity), its idealized [IBD](../../../biology.md#identity-by-descent) [likelihood ratio](../../../statistical-modelling.md#likelihood-ratio) is instead

$$
Z_E(0)=-\log_{10}P(E)=38\log_{10}2-8\log_{10}3\simeq7.622.
$$

This latter value requires the additional negative [genetic marker](../../../biology.md#genetic-marker) observations. It cannot be inferred merely from [homozygosity](../../../biology.md#homozygosity) in the affected subjects, and neither simplified [IBD](../../../biology.md#identity-by-descent) score is an exact identity-by-state [likelihood](../../../statistical-modelling.md#likelihood-function) for an unspecified common [haplotype](../../../biology.md#haplotype).

<h3 id="3/g">g</h3>

↑ **Parent:** [3](#3)

<h4 id="3/g/solution">Solution</h4>

↑ **Parent:** [G](#3/g)

Under the original assumptions the extra affected child is impossible. A generation-3 woman can have at most one copy of the unique introduced disease [allele](../../../biology.md#allele), while an unrelated outside spouse has none. Their children cannot inherit two defective copies. Thus both linkage and no-linkage [likelihoods](../../../statistical-modelling.md#likelihood-function) of the enlarged data are zero, and **the original single-entry model has no defined updated [LOD score](../../../biology.md#lod-score)**. At least one assumption must be relaxed: another introduced disease [allele](../../../biology.md#allele), a new mutation, a phenocopy, or the relationship of the outside spouse.

If the model is enlarged to allow an independent outside [genetic carrier](../../../biology.md#genetic-carrier), the reported extra information contains disease status but no new [genetic marker](../../../biology.md#genetic-marker) [genotypes](../../../biology.md#genotype). In the simple extension with fixed outside heterozygous-carrier [probability](../../../probability-theory.md#probability) $c$, the old disease observations force both generation-2 family ancestors to be [genetic carriers](../../../biology.md#genetic-carrier). A further generation-3 sister inherits the disease copy with [probability](../../../probability-theory.md#probability) $1/2$, independently of the existing offspring transmissions. Given that she and her spouse are [genetic carriers](../../../biology.md#genetic-carrier), exactly one of their three children is affected with [probability](../../../probability-theory.md#probability)

$$
\binom31\frac14\left(\frac34\right)^2=\frac{27}{64}.
$$

The additional [phenotype](../../../biology.md#phenotype) [likelihood](../../../statistical-modelling.md#likelihood-function) is therefore $27c/128$. It is the same at $\theta=0$ and $\theta=1/2$, so it cancels and **the LOD remains unchanged in this phenotype-only, independent-carrier extension**. If the identity of the affected child is specified, the factor is $9c/128$, which also cancels. No such conclusion applies automatically if new [genetic marker](../../../biology.md#genetic-marker) data are supplied or the revised [pedigree founder](../../../biology.md#founder-in-a-pedigree) model couples this branch to the old [genetic marker](../../../biology.md#genetic-marker) evidence.

In general an enlarged data set changes the score by

$$
\Delta Z=\log_{10}\frac{P(\text{new data}\mid\text{old data},\theta=0)}{P(\text{new data}\mid\text{old data},\theta=1/2)},
$$

after choosing a coherent model with positive [likelihood](../../../statistical-modelling.md#likelihood-function). The additional affected child alone does not justify assigning it the [autozygosity](../../../biology.md#autozygosity) evidence of an affected child of a cousin marriage.

## 4

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use standard neutral coalescent time units, so each pair of ancestral lineages merges at rate 1. With $j$ lineages, there are $\binom j2$ possible pairs; consequently the successive waiting times are independent with

$$
T_j\sim\operatorname{Exp}(\lambda_j),\qquad \lambda_j=\frac{j(j-1)}2.
$$

During this epoch there are $j$ branches, each of length $T_j$. Hence the [total branch length of a neutral coalescent](../../../markov-process.md#total-branch-length-of-a-neutral-coalescent) is $L=\sum_{j=2}^n jT_j$, and [linearity of expectation](../../../probability-theory.md#linearity-of-expectation) gives

$$
\boxed{EL=\sum_{j=2}^n\frac{j}{\lambda_j}=2\sum_{i=1}^{n-1}\frac1i.}
$$

The root branch above the sample's common ancestor is excluded: its mutations would be shared by every chromosome and would not be [segregating sites](../../../biology.md#segregating-site) in the sample.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

In the [infinite sites mutation model](../../../biology.md#infinite-sites-mutation-model), mutations occur as independent [Poisson processes](../../../probability-theory.md#poisson-process) at rate $\theta/2$ per lineage per unit of the coalescent time used in part (a). Conditional on the genealogy, superposition over branches gives a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) with mean $\theta L/2$. Since this depends only on $L$, conditioning on total length alone gives

$$
\boxed{S\mid L,\theta\sim\operatorname{Poisson}(\theta L/2).}
$$

Each mutation occurs at a new site and below the common ancestor, so it contributes exactly one [segregating site](../../../biology.md#segregating-site). The [law of iterated expectation](../../../measure-theory.md#law-of-total-expectation) therefore gives, with $a_{n-1}=\sum_{i=1}^{n-1}1/i$,

$$
\boxed{E[S\mid\theta]=\frac\theta2 EL=\theta a_{n-1}.}
$$

Here $\theta$ is fixed when taking the [expectation](../../../probability-theory.md#expected-value). If it is also random under a proper prior with finite mean, the unconditional [expectation](../../../probability-theory.md#expected-value) is $a_{n-1}E\theta$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Assume $n\ge2$, $k\ge0$, a proper [prior density](../../../statistical-inference.md#prior-density) $\pi$ supported on nonnegative mutation rates, and [independence](../../../random-variable.md#independent-random-variables) of the mutation-rate prior from the neutral genealogy. Put

$$
q(t)=\prod_{j=2}^n\lambda_j e^{-\lambda_jt_j}\mathbf1_{\{t_j>0\}},\qquad
L(t)=\sum_{j=2}^n jt_j,\qquad
w_k(\theta,t)=e^{-\theta L(t)/2}\frac{(\theta L(t)/2)^k}{k!}.
$$

By [Bayes' theorem](../../../probability-theory.md#bayes-theorem), the joint posterior is

$$
\boxed{f(\theta,t\mid S=k)=\frac{\pi(\theta)q(t)w_k(\theta,t)}{Z_k},\quad
Z_k=\int_0^\infty\!\pi(u)\int_{(0,\infty)^{n-1}}q(t)w_k(u,t)\,dt\,du.}
$$

The normalizing constant is the prior predictive [probability](../../../probability-theory.md#probability) $P(S=k)$ and must be positive. For $k=0$, interpret the factor $(\theta L/2)^0$ as 1 even at zero. If $n=1$, there are no [segregating sites](../../../biology.md#segregating-site): $S=0$ surely, so that case supplies no information about $\theta$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Use [Bayesian rejection sampling for a segregating-site count](../../../probability-and-statistics.md#bayesian-rejection-sampling-for-a-segregating-site-count). Independently propose $\theta\sim\pi$ and $T_j\sim\operatorname{Exp}(\lambda_j)$ for $j=2,\ldots,n$, and calculate $L=\sum_jjT_j$. Draw an independent uniform $U$ on $(0,1)$ and accept the whole proposed vector exactly when

$$
\boxed{U\le e^{-\theta L/2}\frac{(\theta L/2)^k}{k!}.}
$$

Repeat after a rejection. The right side is a [probability mass function](../../../probability-theory.md#probability-mass-function) value of a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) and is therefore between zero and one. On acceptance, the [probability density function](../../../continuous-probability-distribution.md#probability-density-function) of a proposed vector is its [prior density](../../../statistical-inference.md#prior-density) multiplied by this acceptance [probability](../../../probability-theory.md#probability), divided by the [probability](../../../probability-theory.md#probability) of acceptance. Part (c) shows that this is precisely $f(\theta,T\mid S=k)$. Independent proposals and uniforms produce independent posterior draws. Equivalently, one could simulate a count from a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) with mean $\theta L/2$ and retain the proposal when that count equals $k$; the uniform version avoids simulating that extra count.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

The acceptance [probability](../../../probability-theory.md#probability) is the prior average of the Poisson [likelihood](../../../statistical-modelling.md#likelihood-function):

$$
\boxed{A_k=E_{\theta,T}\left[e^{-\theta L/2}\frac{(\theta L/2)^k}{k!}\right]=Z_k=P_{\rm prior}(S=k).}
$$

Thus the expected number of proposals per accepted draw is $1/Z_k$. A numerical rate depends on the specified prior, sample size and observed count; it is not determined by $k$ alone.

For a more explicit one-dimensional expression, condition on $\theta$. The [probability generating function](../../../probability-theory.md#probability-generating-function), integrating each independent exponential epoch, is

$$
E[z^S\mid\theta]
=E[e^{-\theta(1-z)L/2}]
=\prod_{j=2}^n\frac{\lambda_j}{\lambda_j+\theta j(1-z)/2}
=\prod_{i=1}^{n-1}\frac{i}{i+\theta(1-z)}.
$$

Let $p_k(\theta)$ be its coefficient of $z^k$. Then $Z_k=\int\pi(\theta)p_k(\theta)\,d\theta$. This identifies the acceptance rate with a fully specified marginal [likelihood](../../../statistical-modelling.md#likelihood-function) average.

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

The rejection rule can use a tighter envelope than 1. For $k>0$, differentiate $\log(e^{-x}x^k/k!)=-x+k\log x-\log(k!)$. Its derivative $-1+k/x$ changes from positive to negative at $x=k$, so

$$
M_k=\sup_{x\ge0}e^{-x}\frac{x^k}{k!}=e^{-k}\frac{k^k}{k!},\qquad M_0=1.
$$

Keep the same joint prior proposal but accept with [probability](../../../probability-theory.md#probability) $w_k(\theta,T)/M_k$. Multiplication of the acceptance function by this constant leaves the accepted [probability density function](../../../continuous-probability-distribution.md#probability-density-function) unchanged. The improved rate is

$$
\boxed{A_k^{\rm improved}=\frac{Z_k}{M_k}.}
$$

For $k>0$, $M_k<1$, so this is a genuine improvement; for large $k$, [Stirling's formula](../../../real-analysis.md#stirling-formula) gives $M_k\sim(2\pi k)^{-1/2}$. This is the best global constant envelope for an unrestricted positive prior proposal, because $L$ has support $(0,\infty)$ and $\theta L/2$ can approach $k$. For $k=0$ there is no improvement from this constant scaling. Further gains can come from proposals concentrating near $\theta L/2=k$, or integrating out the times first, but such changes require the appropriate proposal-density ratio and envelope rather than an uncorrected alteration of the sampling law.

<h3 id="4/g">g</h3>

↑ **Parent:** [4](#4)

<h4 id="4/g/solution">Solution</h4>

↑ **Parent:** [G](#4/g)

The accepted mutation parameters have marginal [probability density function](../../../continuous-probability-distribution.md#probability-density-function)

$$
f_\Theta(\theta\mid S=k)=\frac{\pi(\theta)p_k(\theta)}{Z_k}.
$$

Estimate this [probability density function](../../../continuous-probability-distribution.md#probability-density-function) with a suitably smoothed histogram or a boundary-aware [kernel density estimator](../../../nonparametric-statistics.md#kernel-density-estimation) from the accepted draws. On a parameter region where $\pi(\theta)>0$, divide the estimate by the known [prior density](../../../statistical-inference.md#prior-density) and maximize:

$$
\boxed{\widehat\theta_{\rm MC}\in\arg\max_{\theta}\frac{\widehat f_\Theta(\theta\mid S=k)}{\pi(\theta)}.}
$$

The unknown $Z_k$ is constant in $\theta$ and cancels. Maximizing the [posterior density](../../../statistical-inference.md#posterior-density) itself gives a posterior mode, not generally a [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator); the two coincide for a flat prior on a region containing the maximum. A prior excluding candidate maximizers cannot recover them through its posterior output. Boundary behavior also matters: for $k=0$, the [likelihood](../../../statistical-modelling.md#likelihood-function) is decreasing in $\theta$, so the unrestricted maximum is at $\theta=0$.

The exact [likelihood](../../../statistical-modelling.md#likelihood-function) provides a useful independent check. Put $W=L/2$. Its [Laplace transform](../../../analysis.md#laplace-transform) is $\prod_{i=1}^{n-1}i/(i+s)$, since $jT_j/2$ is exponential of rate $j-1$. The [probability density function](../../../continuous-probability-distribution.md#probability-density-function)

$$
g_W(w)=(n-1)e^{-w}(1-e^{-w})^{n-2},\qquad w>0,
$$

has that same transform: substitute $u=e^{-w}$ to obtain $(n-1)\int_0^1u^s(1-u)^{n-2}du=\prod_{i=1}^{n-1}i/(i+s)$. Thus, expanding its binomial factor and integrating each term,

$$
p_k(\theta)=\frac{\theta^k}{k!}\int_0^\infty w^ke^{-\theta w}g_W(w)dw
=(n-1)\theta^k\sum_{r=0}^{n-2}\frac{(-1)^r\binom{n-2}{r}}{(\theta+r+1)^{k+1}}.
$$

This is the [segregating-site likelihood under the neutral coalescent](../../../biology.md#segregating-site-likelihood-under-the-neutral-coalescent). It can be maximized numerically to check the posterior-density estimate; the generating-function representation avoids cancellation in large alternating sums. For $n=2$, it reduces to $\theta^k/(1+\theta)^{k+1}$, whose maximum is at $\theta=k$ for $k>0$.

Alternatively, differentiating the integrated [likelihood](../../../statistical-modelling.md#likelihood-function) gives

$$
\frac{d}{d\theta}\log p_k(\theta)=\frac{k}{\theta}-E[W\mid S=k,\theta].
$$

An interior maximum therefore satisfies $\theta=k/E[W\mid S=k,\theta]$. [Conditional expectations](../../../measure-theory.md#conditional-expectation) of $W$ can be estimated by smoothing the accepted pairs $(\theta,W)$ near each candidate parameter value, yielding another simulation-based score equation. The simple estimator $k/a_{n-1}$ is the unbiased [Watterson estimator](../../../biology.md#watterson-estimator) from part (b), and is not generally the [likelihood](../../../statistical-modelling.md#likelihood-function) maximizer.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
