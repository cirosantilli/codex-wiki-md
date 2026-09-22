<h1 id="8/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $M$ count the ringed birds among the two captures, and let $D$ be the [event](../../../../../../event.md) that the detector records at least one ring. The [hypergeometric distribution](../../../../../../hypergeometric-distribution.md) gives the [prior probabilities](../../../../../../prior-probability.md)

$$
\mathbb P(M=0)=\frac{\binom62}{\binom{10}2}=\frac13,\quad
\mathbb P(M=1)=\frac{4\cdot6}{\binom{10}2}=\frac8{15},\quad
\mathbb P(M=2)=\frac{\binom42}{\binom{10}2}=\frac2{15}.
$$

Under the usual additional assumption of [independent](../../../../../../independent-random-variables.md) per-ring detection, with no false records, the [likelihoods](../../../../../../likelihood-function.md) $\mathbb P(D\mid M=m)$ are $0$, $9/10$, and $1-(1/10)^2=99/100$. Therefore $\mathbb P(D)=12/25+33/250=153/250$. Applying [Bayes' theorem](../../../../../../bayes-theorem.md) yields **$\displaystyle\mathbb P(M=0\mid D)=0,\quad\mathbb P(M=1\mid D)=\frac{40}{51},\quad\mathbb P(M=2\mid D)=\frac{11}{51}$**. Storing only the last detected number means that a stored record does not identify how many rings were present. By label symmetry, the identity of that stored ring does not further alter this distribution.

The text specifies each ring's marginal detection [probability](../../../../../../probability.md), but does not explicitly specify [independence](../../../../../../independent-random-variables.md) of the detection errors. To keep this modelling qualification visible, let $\ell=\mathbb P(D\mid M=2)$. The marginal detection rate only implies $9/10\leq\ell\leq1$. Without the extra [independence](../../../../../../independent-random-variables.md) assumption, the full family of possible [posterior distributions](../../../../../../bayesian-posterior.md) is

$$
\mathbb P(M=0\mid D)=0,\qquad
\mathbb P(M=1\mid D)=\frac{18/5}{18/5+\ell},\qquad
\mathbb P(M=2\mid D)=\frac{\ell}{18/5+\ell}.
$$

In particular $1/5\leq\mathbb P(M=2\mid D)\leq5/23$. The displayed numerical answer corresponds to $\ell=99/100$; the general answer exposes exactly what the detector's marginal specification alone establishes.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics, and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
