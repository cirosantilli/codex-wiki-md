<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $b^1_{\ell_1\ell_2\ell_3}$ denote the template at unit $f_{\mathrm{NL}}$, and define $A_{123}=b^1_{\ell_1\ell_2\ell_3}\mathcal G_{m_1m_2m_3}^{\ell_1\ell_2\ell_3}$. All sums below are over ordered triples of the retained multipoles, with the monopole removed and $C_\ell>0$. A finite maximum multipole makes these expressions ordinary finite sums. Taking the expectation of the cubic numerator and using the template relation gives

$$
\langle\hat f_{\mathrm{NL}}\rangle=\frac{f_{\mathrm{NL}}}{6F}
\sum_{123}\frac{A_{123}^2}{C_{\ell_1}C_{\ell_2}C_{\ell_3}}.
$$

Thus the [full-sky cubic bispectrum estimator](../../../../../../full-sky-cubic-bispectrum-estimator.md) is unbiased for

$$
\boxed{F=\frac16\sum_{\ell_1m_1,\ell_2m_2,\ell_3m_3}
\frac{(b^1_{\ell_1\ell_2\ell_3})^2(\mathcal G_{m_1m_2m_3}^{\ell_1\ell_2\ell_3})^2}
{C_{\ell_1}C_{\ell_2}C_{\ell_3}}.}
$$

The assumed template must have nonzero support, so $F>0$. Using the Gaunt sum rule, write

$$
h_{\ell_1\ell_2\ell_3}^2=\frac{(2\ell_1+1)(2\ell_2+1)(2\ell_3+1)}{4\pi}
\begin{pmatrix}\ell_1&\ell_2&\ell_3\\0&0&0\end{pmatrix}^{\!2},\qquad
\boxed{F=\frac16\sum_{\ell_1\ell_2\ell_3}\frac{h_{\ell_1\ell_2\ell_3}^2(b^1_{\ell_1\ell_2\ell_3})^2}{C_{\ell_1}C_{\ell_2}C_{\ell_3}}.}
$$

The factor $1/6$ belongs to the ordered sum; an unordered triangle sum would instead use multiplicity factors for equal multipoles. This normalization is also the Gaussian [Fisher information](../../../../../../fisher-information-matrix.md) for the template amplitude.

For the [cosmic variance](../../../../../../cosmic-variance.md), use the reality condition $\Theta_{\ell m}^*=(-1)^m\Theta_{\ell,-m}$ and Gaussian covariance

$$
\langle\Theta_{\ell m}\Theta_{\ell'm'}\rangle
=(-1)^mC_\ell\delta_{\ell\ell'}\delta_{m,-m'}.
$$

There are $15$ pairings of the six multipoles in the squared cubic numerator. Six pairings connect every factor in the first triple to a factor in the second. Each gives $\sum A_{123}^2/(C_{\ell_1}C_{\ell_2}C_{\ell_3})=6F$. The covariance phases cancel: nonzero [Gaunt integrals](../../../../../../gaunt-integral.md) have $m_1+m_2+m_3=0$, and simultaneous reversal of the three $m$ indices multiplies the Gaunt integral by $(-1)^{\ell_1+\ell_2+\ell_3}=1$.

The other nine pairings contain one contraction within each triple. To see why their sums vanish, contract two legs of a Gaunt integral and use the [spherical harmonic addition theorem](../../../../../../spherical-harmonic-addition-theorem.md):

$$
\sum_m(-1)^m\mathcal G^{\ell\ell L}_{m,-m,M}
=\int d\hat n\,Y_{LM}(\hat n)\sum_m|Y_{\ell m}(\hat n)|^2
=\frac{2\ell+1}{4\pi}\int d\hat n\,Y_{LM}(\hat n)=0\quad(L>0).
$$

The template and inverse-covariance weights are independent of $m$, so they do not spoil this cancellation. The only possible surviving unpaired mode is the monopole, and $\Theta_{00}=0$ removes it. This is [monopole cancellation of internal cubic-estimator contractions](../../../../../../monopole-cancellation-of-internal-cubic-estimator-contractions.md). It explains why no linear correction is needed in this ideal full-sky isotropic problem; masks or anisotropic noise would spoil the argument.

The cubic numerator therefore has Gaussian variance $6(6F)=36F$. Dividing by $(6F)^2$ gives

$$
\boxed{\operatorname{Var}_{f_{\mathrm{NL}}=0}(\hat f_{\mathrm{NL}})=\frac1F,\qquad
\sigma(f_{\mathrm{NL}})=F^{-1/2}.}
$$

The result concerns the Gaussian-limit covariance. Non-Gaussian connected four- and six-point terms can change the variance at finite amplitude. Unbiasedness uses the assumed linear template relation for the observed three-point function.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
