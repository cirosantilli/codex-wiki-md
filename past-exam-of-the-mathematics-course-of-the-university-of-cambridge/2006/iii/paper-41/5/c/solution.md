<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the missing strong-swimmer times $U_j=S_{j1}$, $j=4,\ldots,8$, as the [latent variables](../../../../../../latent-variable.md). Their partners' times are $T_j-U_j$. The complete-data [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell_c=8\log\lambda_1+8\log\lambda_2
-\lambda_1\left(A+\sum_{j=4}^8U_j\right)
-\lambda_2\left(B+\sum_{j=4}^8(T_j-U_j)\right).
$$

For the E-step of the [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md), use the [conditional split of two exponential times](../../../../../../conditional-split-of-two-exponential-times.md). At the old rates, with $d_r=\lambda_1^{(r)}-\lambda_2^{(r)}>0$,

$$
f(u\mid T_j=t)=\frac{d_re^{-d_ru}}{1-e^{-d_rt}},\qquad0<u<t.
$$

This is a [truncated exponential distribution](../../../../../../truncated-exponential-distribution.md), whose [conditional expectation](../../../../../../conditional-expectation.md) is

$$
\boxed{m_j^{(r)}=E[U_j\mid T_j,\theta^{(r)}]
=\frac1{d_r}-\frac{T_j}{e^{d_rT_j}-1}.}
$$

The displayed mean follows by integrating $u e^{-d_ru}$ against the conditional density; the missing weak-swimmer mean is $T_j-m_j^{(r)}$. As $d_r\to0$, the conditional density becomes uniform on $(0,T_j)$ and $m_j^{(r)}\to T_j/2$.

Write $U_r=A+\sum_jm_j^{(r)}$ and $V_r=B+\sum_j(T_j-m_j^{(r)})$. The E-step objective is

$$
Q=8\log\lambda_1+8\log\lambda_2-\lambda_1U_r-\lambda_2V_r.
$$

Setting its [partial derivatives](../../../../../../partial-derivative.md) to zero gives the unconstrained M-step

$$
\boxed{\lambda_1^{(r+1)}=\frac8{U_r},\qquad
\lambda_2^{(r+1)}=\frac8{V_r}.}
$$

These are eight divided by the completed expected totals for the corresponding swimmers; imputing only observed pair totals without the conditional split would not perform the E-step.

The stated ordering must also be enforced. The [ordered-rate exponential M-step](../../../../../../ordered-rate-exponential-m-step.md) accepts these updates when $U_r<V_r$, so $\lambda_1^{(r+1)}>\lambda_2^{(r+1)}$. Otherwise its maximum on the closed constraint $\lambda_1\geq\lambda_2$ lies at

$$
\boxed{\lambda_1^{(r+1)}=\lambda_2^{(r+1)}
=\frac{16}{U_r+V_r}
=\frac{16}{A+B+\sum_{j=4}^8T_j}.}
$$

Under a strictly open constraint $\lambda_1>\lambda_2$, a boundary optimum is only a supremum; a finite interior maximizer is not assured for every possible sample. One should report that situation rather than swap the labeled swimmer groups. Starting from positive ordered rates, iterate the E-step and constrained M-step until the parameter changes and observed [log-likelihood](../../../../../../log-likelihood.md) improvement are small. [EM likelihood monotonicity](../../../../../../em-likelihood-monotonicity.md) applies to every exact constrained M-step. No numerical swimming times are supplied, so the data-dependent updates, rather than fabricated numerical estimates, are the answer.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
