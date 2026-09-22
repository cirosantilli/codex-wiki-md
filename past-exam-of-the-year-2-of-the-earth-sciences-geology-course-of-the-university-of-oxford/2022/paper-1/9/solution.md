<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Test **homogeneity of the four category [probabilities](../../../../probability.md)** among the three samples. The [null hypothesis](../../../../null-hypothesis.md) is $p_{iA}=p_{iB}=p_{iC}$ for every category $i$; the alternative allows at least one difference. This is a [Pearson chi-squared test of homogeneity](../../../../pearson-chi-squared-test-of-homogeneity.md), assuming independently sampled grains with consistent classification.

The row totals are $(195,52,64,16)$, the sample totals $(131,135,61)$ and the grand total $N=327$. Under the [null hypothesis](../../../../null-hypothesis.md), $E_{ij}=O_{i+}O_{+j}/N$, giving the [expected value](../../../../expected-value-split.md) table

$$
\begin{array}{c|rrr}
& A&B&C\\\hline
\text{non-undulatory}&78.1193&80.5046&36.3761\\
\text{undulatory}&20.8318&21.4679&9.7003\\
\text{polycrystalline, 2–3}&25.6391&26.4220&11.9388\\
\text{polycrystalline, greater than 3}&6.4098&6.6055&2.9847
\end{array}
$$

For example, $E_{\mathrm{undulatory},C}=52(61)/327=9.7003$, so that cell contributes $(4-9.7003)^2/9.7003=3.34974$. The complete cell contributions are

$$
\frac{(O-E)^2}{E}=
\begin{pmatrix}
0.217211&0.003049&0.361014\\
0.481834&0.298659&3.349738\\
0.217388&0.222018&0.000313\\
0.310072&0.055505&1.360734
\end{pmatrix},
$$

so **$X^2=6.87754$**. There are $(4-1)(3-1)=6$ [statistical degrees of freedom](../../../../statistical-degrees-of-freedom.md). The supplied $5\%$ critical value is $12.592$, and $6.87754<12.592$, so **do not reject homogeneity at $\alpha=0.05$**. The approximate upper-tail [p-value](../../../../p-value.md) is $0.3323$.

One of twelve expected cells is below five, with none below one; the asymptotic approximation is broadly defensible by a common expected-count guideline but is not exact. An exact/conditional simulation could check it, especially if grain counts are clustered. Do not pool categories solely to obtain a desired result. The conclusion is that these counts do not demonstrate different category proportions; **they do not prove that the rocks share one [geological formation](../../../../geological-formation.md)**. Different formations can share such proportions, and real grains within one rock can fail the independent-sampling assumption.

## ↑ Ancestors (11)

1. [9](../9.md)
2. [Paper 1](../../paper-1-split.md)
3. [2022](../../split.md)
4. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../split.md)
5. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
6. [Earth sciences (geology) course of the University of Oxford](../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
