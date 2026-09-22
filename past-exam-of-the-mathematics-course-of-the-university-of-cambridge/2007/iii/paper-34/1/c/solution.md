<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Omit indices of probability zero. The [support of a positive operator](../../../../../../support-of-a-positive-operator.md) of every remaining $\rho_i$ lies within that of $\overline\rho$, because $\overline\rho$ is a positive sum containing $p_i\rho_i$. Thus $D(\rho_i\Vert\overline\rho)$ is finite.

First suppose $\operatorname{supp}\overline\rho\subseteq\operatorname{supp}\sigma$, so all quantities are finite. Expand the trace definitions of [quantum relative entropy](../../../../../../quantum-relative-entropy.md):

$$
\begin{aligned}
\sum_ip_iD(\rho_i\Vert\sigma)-\sum_ip_iD(\rho_i\Vert\overline\rho)
&=\sum_ip_i\operatorname{Tr}\rho_i(\log_2\overline\rho-\log_2\sigma)\\
&=\operatorname{Tr}\overline\rho(\log_2\overline\rho-\log_2\sigma)\\
&=D(\overline\rho\Vert\sigma).
\end{aligned}
$$

Therefore [Donald's identity](../../../../../../donald-s-identity.md) is

$$
\boxed{\sum_ip_iD(\rho_i\Vert\sigma)=\sum_ip_iD(\rho_i\Vert\overline\rho)+D(\overline\rho\Vert\sigma).}
$$

If the support condition on $\sigma$ fails, at least one positive-weight $\rho_i$ also fails it. The left side and the final term on the right are then $+\infty$, while the first right-hand sum remains finite. The equality is valid in this extended sense, without taking any undefined difference of infinities.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
