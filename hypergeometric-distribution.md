# Hypergeometric distribution

↑ **Parent:** [Discrete probability distribution](discrete-probability-distribution-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hypergeometric_distribution)

The [hypergeometric distribution](hypergeometric-distribution.md) counts marked objects in a uniformly chosen sample of fixed size from a finite population, using [sampling without replacement](sampling-without-replacement.md). Let $n\geq1$ be the population size, let $0\leq c\leq n$ objects be marked, and sample $0\leq r\leq n$ distinct objects. If $K$ counts the marked objects selected, its [probability mass function](probability-mass-function.md) is

$$
\mathbb P(K=k)=\frac{\binom ck\binom{n-c}{r-k}}{\binom nr},
\qquad \max(0,r-(n-c))\leq k\leq\min(c,r).
$$

The bounds describe the [support of a probability distribution](support-of-a-probability-distribution.md) and $k$ must be an [integer](integer-split.md); the mass is zero elsewhere. The denominator counts all size-$r$ [subsets](subset.md), while the numerator counts choices of $k$ marked and $r-k$ unmarked objects using [binomial coefficients](binomial-coefficient-split.md). This counting argument requires every size-$r$ sample to have the same [probability](probability.md).[MIT 14.30, hypergeometric distribution handout, §§1–4](https://web.mit.edu/14.380/www/handouts/hypergeometric.pdf)

For a constructed example, a box contains ten labelled objects, four red and six blue. Select five without replacement. There are $\binom{10}{5}=252$ possible samples. The [probabilities](probability.md) for $K=0,1,2,3,4$ are

$$
\frac1{42},\quad\frac5{21},\quad\frac{10}{21},\quad\frac5{21},\quad\frac1{42}.
$$

In particular, $\mathbb P(K=2)=\binom42\binom63/252=120/252=10/21$. Five red objects are impossible because the box only contains four. The [expected value](expected-value-split.md) is $r(c/n)=2$, and the [variance](variance-split.md) is $2/3$.

<a id="image-five-draws-from-four-red-and-six-blue-objects-replacement-preserves-the-mean-but-changes-the-spread"></a>
![](hypergeometric-versus-binomial.png)

**[Figure 10](#image-five-draws-from-four-red-and-six-blue-objects-replacement-preserves-the-mean-but-changes-the-spread). Five draws from four red and six blue objects: replacement preserves the mean but changes the spread**.

The count law also answers a detection question: what is the chance that five draws find at least one red object? By the [complement rule of probability](complement-rule-of-probability.md), it is $1-\mathbb P(K=0)=41/42$, approximately $0.9762$. This can model inspecting five distinct objects from a known finite collection, with a mark indicating the property we want to detect. If repeated inspections can select the same object again, the replacement model instead gives $1-0.6^5=0.92224$. Equal [expected values](expected-value-split.md) therefore do not imply equal chances of detecting a marked object.

The corresponding [binomial distribution](binomial-distribution.md) counts red draws when each selected object is put back before the next independent draw: $K_{\mathrm{rep}}\sim\operatorname{Bin}(5,0.4)$. It has the same [expected value](expected-value-split.md) $2$, but [variance](variance-split.md) $5(0.4)(0.6)=6/5$, and it permits five red draws. Without replacement, a red first draw leaves red [probability](probability.md) $3/9$ for the next draw; a blue first draw leaves $4/9$. This [statistical dependence](statistical-dependence.md) pulls the total toward the fixed composition of the population, producing the [finite population correction](finite-population-correction.md).

The useful modelling question is whether previously selected objects remain available. A fixed-size sample of distinct items calls for a [hypergeometric distribution](hypergeometric-distribution.md); fresh independent trials with constant success [probability](probability.md) call for a [binomial distribution](binomial-distribution.md). When the population grows with $c/n\to p$ while $r$ stays fixed, the hypergeometric masses tend to the corresponding [binomial distribution](binomial-distribution.md) masses: removing finitely many objects has an increasingly small effect on the next draw's [probability](probability.md).

**Table of contents**

- [Finite population correction](finite-population-correction.md)
- [Multivariate hypergeometric distribution](multivariate-hypergeometric-distribution.md)

## ↑ Ancestors (7)

1. [Discrete probability distribution](discrete-probability-distribution-split.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (29)

- [Binomial distribution](binomial-distribution.md)
- [Capture-recapture model](capture-recapture-model.md)
- [Closed-population capture-recapture model](closed-population-capture-recapture-model.md)
- [Complement rule of probability](complement-rule-of-probability.md)
- [Conditional composition of two independent binomial counts](conditional-composition-of-two-independent-binomial-counts.md)
- [Cyclic interval overlap bound](cyclic-interval-overlap-bound.md)
- [Exact power of Fisher's exact test](exact-power-of-fisher-s-exact-test.md)
- [Finite population correction](finite-population-correction.md)
- [Hypergeometric allocation of exchangeable Bernoulli counts](hypergeometric-allocation-of-exchangeable-bernoulli-counts.md)
- [Hypergeometric distribution](hypergeometric-distribution.md)
- [Multivariate hypergeometric distribution](multivariate-hypergeometric-distribution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-37/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-44/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-36/1/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-207/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-221/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-221/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2/section-a/9/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-2/11/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-2/11/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/18/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1/18/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1/18/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/16/a/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/16/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/16/c/ii/solution.md)
- [Sampling without replacement](sampling-without-replacement.md)
- [Sampling without replacement need not be independent](sampling-without-replacement-need-not-be-independent.md)
