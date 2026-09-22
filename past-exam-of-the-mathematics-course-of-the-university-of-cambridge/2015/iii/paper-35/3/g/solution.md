<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The [expected values](../../../../../../expected-value.md) of early and late new diagnosis counts at step $k$ are

$$
e_k=\delta_Eh_{k-1}(\theta),\qquad
n_k=\delta_N(1-\delta_E)\sum_{i=1}^{k-2}
 h_i(\theta)(1-\delta_N)^{k-i-2}.
$$

Each summand in $n_k$ corresponds to an infection that avoids early diagnosis, enters the non-early state one step later, remains there for the intervening steps and is then diagnosed. Define $h_j=0$ for $j\leq0$, and take an empty sum as zero. **The early share of diagnosis intensity is**

$$
\boxed{p_{Ek}=\frac{e_k}{e_k+n_k}
=\frac{\delta_Eh_{k-1}(\theta)}{\delta_Eh_{k-1}(\theta)
+\delta_N(1-\delta_E)\sum_{i=1}^{k-2}h_i(\theta)(1-\delta_N)^{k-i-2}}.}
$$

It is defined only when $e_k+n_k>0$; in particular there are no diagnoses at step 1 under the initial condition. With infection counts following a [Poisson distribution](../../../../../../poisson-distribution.md) and independent marking, early and late diagnosis counts in a fixed interval are [independent](../../../../../../independent-random-variables.md) [Poisson random variables](../../../../../../poisson-distribution.md). Conditional on a positive total, the early count has a [binomial distribution](../../../../../../binomial-distribution.md) given the total with probability $p_{Ek}$, so this ratio also equals the [expectation](../../../../../../expected-value.md) of the observed early fraction conditional on a nonzero total. Without that conditioning a sample fraction at zero diagnoses is undefined.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
