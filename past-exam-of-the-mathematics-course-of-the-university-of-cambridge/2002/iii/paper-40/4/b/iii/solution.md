<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The E-step uses the posterior class [probabilities](../../../../../../../probability.md)

$$
\boxed{w_{ij}^{(m)}=\frac{\alpha_j^{(m)}f_j(x_i;\mu_j^{(m)},v^{(m)})}{\sum_{r=1}^2\alpha_r^{(m)}f_r(x_i;\mu_r^{(m)},v^{(m)})}.}
$$

Let $n_j^{(m)}=\sum_iw_{ij}^{(m)}$, so $n_1^{(m)}+n_2^{(m)}=n$. Up to constants, the expected complete-data [log-likelihood](../../../../../../../log-likelihood.md) is

$$
Q=\sum_jn_j^{(m)}\log\alpha_j-\frac n2\log v-\frac1{2v}\sum_{i,j}w_{ij}^{(m)}(x_i-\mu_j)^2.
$$

Maximizing the first term with $\alpha_1+\alpha_2=1$ gives $\alpha^{(m+1)}=n_1^{(m)}/n$. Differentiating in each $\mu_j$ gives $\mu_j^{(m+1)}=\sum_iw_{ij}^{(m)}x_i/n_j^{(m)}$. After these updates, maximizing in the shared [variance](../../../../../../../variance-split.md) gives

$$
\boxed{v^{(m+1)}=\frac1n\sum_{i=1}^n\sum_{j=1}^2w_{ij}^{(m)}\left(x_i-\mu_j^{(m+1)}\right)^2.}
$$

The residuals use the new component means, while the weights remain from the old parameters. The divisor is $n$, not $n-2$, because this is a maximum-likelihood update. Starting with $0<\alpha<1$ and $v>0$ gives positive responsibilities and positive $n_j$; a zero effective component size at a boundary would leave its mean unidentified. These are the [EM for Gaussian mixtures with a common variance](../../../../../../../em-for-gaussian-mixtures-with-a-common-variance.md) transitions.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
