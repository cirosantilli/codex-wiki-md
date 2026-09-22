<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\overline\omega=\sum_jp_j\omega_j$. When the relative entropies are finite, expanding their trace definitions gives

$$
\begin{aligned}
\sum_jp_jD(\omega_j\|\rho)-\sum_jp_jD(\omega_j\|\overline\omega)
&=\sum_jp_j\operatorname{Tr}[\omega_j(\log_2\overline\omega-\log_2\rho)]\\
&=\operatorname{Tr}[\overline\omega(\log_2\overline\omega-\log_2\rho)]
=D(\overline\omega\|\rho).
\end{aligned}
$$

Thus [Donald's identity](../../../../../../donald-s-identity.md) is

$$
\boxed{\sum_jp_jD(\omega_j\|\rho)
=\sum_jp_jD(\omega_j\|\overline\omega)+D(\overline\omega\|\rho)}.
$$

For every $p_j>0$, the [support of a positive operator](../../../../../../support-of-a-positive-operator.md) $\omega_j$ lies in that of $\overline\omega$, so the first sum on the right is finite in finite dimension. If the support of $\overline\omega$ is not contained in the support of $\rho$, at least one positive-weight $\omega_j$ also violates the support condition. Both sides of the identity are then $+\infty$. This extends the conclusion without subtracting infinite quantities.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
