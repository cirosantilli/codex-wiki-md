<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

Treat the two row totals as fixed sample sizes, with independent multinomial observations within each row. More generally let $N_{ij}$ be an $r$ by $c$ table, row totals $n_i$, column totals $m_j$ and total $N$. Under the unrestricted alternative, row $i$ has its own category probabilities $p_{ij}$; independence means that all rows have the same probabilities $p_j$.

Ignoring the multinomial coefficients, which cancel in a likelihood ratio, the unrestricted likelihood is $\prod_{ij}p_{ij}^{N_{ij}}$. Maximizing $\sum_jN_{ij}\log p_{ij}$ under $\sum_jp_{ij}=1$ gives $\widehat p_{ij}=N_{ij}/n_i$. Under the null, the log likelihood is $\sum_jm_j\log p_j$, giving $\widehat p_j=m_j/N$. Thus the null fitted counts are $E_{ij}=n_im_j/N$, and the generalized likelihood ratio is

$$
\Lambda=\frac{\sup_{H_0}L}{\sup L}=\prod_{ij}\left(\frac{E_{ij}}{N_{ij}}\right)^{N_{ij}},\qquad\boxed{G^2=-2\log\Lambda=2\sum_{ij}N_{ij}\log\frac{N_{ij}}{E_{ij}}}.
$$

A zero observed count contributes zero by [continuity](../../../../../continuous-function.md). Small $\Lambda$, equivalently large $G^2$, is evidence against independence. The unrestricted model has $r(c-1)$ free probabilities and the null has $c-1$, a difference of $(r-1)(c-1)$. Under the usual large-sample likelihood-ratio approximation at an interior null, $G^2$ has a [chi-squared distribution](../../../../../chi-squared-distribution.md) with that many degrees of freedom. This is the [likelihood-ratio test of independence in a contingency table](../../../../../likelihood-ratio-test-of-independence-in-a-contingency-table.md). Sampling the entire table multinomially instead gives the same statistic and degrees of freedom after estimating the row probabilities.

For the supplied data the fitted counts are

$$
E=\begin{pmatrix}15&25&10\\45&75&30\end{pmatrix}.
$$

Substitution gives

$$
G^2=2\left[17\log\frac{17}{15}+22\log\frac{22}{25}+11\log\frac{11}{10}+43\log\frac{43}{45}+78\log\frac{78}{75}+29\log\frac{29}{30}\right]\simeq0.9701.
$$

There are $(2-1)(3-1)=2$ degrees of freedom. The supplied 1% critical value is $9.21$, and $0.9701<9.21$. **Do not reject independence at the 0.01 level.** The approximate chi-squared tail probability is $e^{-G^2/2}\simeq0.616$. This lack of rejection does not establish that the classifications are independent; the test supplies no evidence against that null here. All fitted counts are at least ten, making the stated asymptotic approximation reasonable.

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
