<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
\bar q=\frac1K\sum_{k=1}^Kq_k,
\qquad
\bar x=\frac1N\sum_{i=1}^Nx_i,
$$

and set

$$
A=\operatorname{Var}(\bar q)
=\sigma_\mu^2+\sigma_G^2+\frac{\sigma_I^2}{K},
\qquad
B=\operatorname{Var}(\bar x)
=\frac{\sigma_{\rm tot}^2}{N}.
$$

The within-galaxy contrasts $q_k-\bar q$ contain no $M_0$, so the parameter-dependent [log-likelihood](../../../../../../log-likelihood.md) reduces to

$$
\ell(M_0,\theta)
=-\frac{(\bar q-M_0)^2}{2A}
-\frac{\{\bar x-(M_0-\theta)\}^2}{2B}+\text{constant}.
$$

The [score equations](../../../../../../score-equation.md) give the [maximum-likelihood estimators](../../../../../../maximum-likelihood-estimator.md)

$$
\widehat M_0=\bar q,
\qquad
\widehat\theta=\bar q-\bar x.
$$

The calibrator and Hubble-flow samples are independent, so both estimators are [unbiased](../../../../../../unbiased-estimator.md) and

$$
\operatorname{Var}(\widehat M_0)=A,
\qquad
\operatorname{Var}(\widehat\theta)=A+B.
$$

The [Fisher information matrix](../../../../../../fisher-information-matrix.md) for $(M_0,\theta)$ is

$$
\mathcal I=
\begin{pmatrix}
A^{-1}+B^{-1}&-B^{-1}\\
-B^{-1}&B^{-1}
\end{pmatrix},
\qquad
\mathcal I^{-1}=
\begin{pmatrix}
A&A\\
A&A+B
\end{pmatrix}.
$$

**Hence $\operatorname{Var}(\widehat\theta)=(\mathcal I^{-1})_{22}$: $\widehat\theta$ attains the multiparameter [Cramér-Rao bound](../../../../../../cramer-rao-bound.md).**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
