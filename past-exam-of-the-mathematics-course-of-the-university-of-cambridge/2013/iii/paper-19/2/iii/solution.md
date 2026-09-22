<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First the increasing sequence is cofinal in $\kappa$. Write $\mu=\sup_{\xi<\delta}\kappa_\xi$. Strict increase gives $|\delta|\le\mu$ when the sequence is infinite, so its [cardinal](../../../../../../cardinal-number.md) sum is $\max(|\delta|,\mu)=\mu$. The given sum therefore implies $\mu=\kappa$ and $|\delta|\le\kappa$.

For any [function](../../../../../../function-split.md) $f:\lambda\to\kappa$, choose an index $\xi_t$ with $f(t)<\kappa_{\xi_t}$ for every $t<\lambda$. There are at most $\lambda<\operatorname{cf}(\delta)$ such indices, so they are bounded below $\delta$. Enlarging the bound if needed gives an index $\xi$ with $\operatorname{ran}(f)\subseteq\kappa_\xi$. Thus

$$
{}^\lambda\kappa=\bigcup_{\xi<\delta}{}^\lambda\kappa_\xi,
\qquad \kappa^\lambda\le\sum_{\xi<\delta}\kappa_\xi^\lambda.
$$

Conversely each summand is at most $\kappa^\lambda$, and $|\delta|\le\kappa\le\kappa^\lambda$ because $\lambda\ne0$. Infinite [cardinal](../../../../../../cardinal-number.md) multiplication consequently gives

$$
\sum_{\xi<\delta}\kappa_\xi^\lambda
\le|\delta|\cdot\kappa^\lambda=\kappa^\lambda.
$$

Combining the inequalities proves **$\kappa^\lambda=\sum_{\xi<\delta}\kappa_\xi^\lambda$**.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
