<h1 id="13j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Model 2 is obtained from model 3 by setting $\beta_0=0$. Model 3 is contained in model 1 by choosing the symmetric block parameters

$$
\beta_{k\ell}^{(1)}=
\begin{cases}
\beta_k+\beta_\ell,&k\ne\ell,\\
2\beta_k+\beta_0,&k=\ell.
\end{cases}
$$

Hence

$$
\boxed{\text{model 2}\subset\text{model 3}\subset\text{model 1}.}
$$

Assuming every college-pair cell is observed and the models are identifiable, model 1 has $C(C+1)/2$ parameters and model 3 has $C+1$. The [likelihood-ratio test statistic](../../../../../../likelihood-ratio-test-statistic.md) for model 3 against model 1 is

$$
D=2\{\ell_1(\widehat\beta_1)-\ell_3(\widehat\beta_3)\}.
$$

Under model 3 and the regularity conditions of [Wilks theorem](../../../../../../wilks-theorem.md),

$$
\boxed{D\ \xrightarrow{d}\ \chi^2_{\,C(C+1)/2-(C+1)}
=\chi^2_{(C-2)(C+1)/2}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [13J](../../13j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
