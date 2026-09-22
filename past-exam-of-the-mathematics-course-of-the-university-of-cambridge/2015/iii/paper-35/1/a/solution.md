<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $C$ for the binary response, $P$ for the partner count, and $Z$ for fully observed background variables. Let $R=(R_C,R_P)$ indicate which of $C,P$ are observed, with 1 meaning observed. For any realised pattern $r$, partition the data into $D_{\mathrm{obs}}(r)$ and $D_{\mathrm{mis}}(r)$.

[Missing completely at random](../../../../../../missing-completely-at-random.md) means that the [missing-data mechanism](../../../../../../missing-data-mechanism.md) does not depend on any of the measurements:

$$
\boxed{\Pr(R=r\mid C,P,Z)=\Pr(R=r).}
$$

[Missing at random](../../../../../../missing-at-random.md) allows dependence on the data observed under the particular pattern, but no further dependence on its unobserved values:

$$
\boxed{\Pr(R=r\mid D_{\mathrm{obs}},D_{\mathrm{mis}})=\Pr(R=r\mid D_{\mathrm{obs}}).}
$$

Thus a response probability depending on fully observed age or sex can satisfy [missing at random](../../../../../../missing-at-random.md). Dependence on an observed partner count can also be permissible for patterns in which that count is available. [Missing not at random](../../../../../../missing-not-at-random.md) means that this equality fails: the probability of the pattern still depends on one of its missing measurements, after conditioning on the observed ones. **The distinction concerns dependence on the unseen values, not whether missingness looks haphazard.** These definitions can be applied within the target population $P>1$; unknown membership of that population must itself be handled when $P$ is missing.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
