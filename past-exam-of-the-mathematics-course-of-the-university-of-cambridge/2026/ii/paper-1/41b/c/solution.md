<h1 id="41b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $q^{(0)}=\sum_i c_iq_i$ with $c_1\ne0$. After $k$ multiplications, the tangent of the angle to $q_1$ is at most

$$
\frac{\sqrt{\sum_{i\ge2}c_i^2|\lambda_i|^{2k}}}
{|c_1||\lambda_1|^k}
\le\left|\frac{\lambda_2}{\lambda_1}\right|^k\tan\theta_0.
$$

Since $|\sin\theta_k|\le\tan\theta_k$, the first bound follows. Also

$$
\lambda^{(k)}-\lambda_1
=\sum_{i\ge2}(\lambda_i-\lambda_1)|q_i^Tq^{(k)}|^2.
$$

Bound the coefficient by $\max_{i\ge2}|\lambda_i-\lambda_1|$ and the sum by $\sin^2\theta_k$, then use the squared first estimate to obtain the second bound.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [41B](../../41b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
