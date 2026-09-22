<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $q_\phi=N(\mu_Q,\sigma_Q^2)$,

$$
\operatorname{ELBO}(\mu_Q,\sigma_Q^2)
=-\frac12\log(2\pi\sigma^2)
-\frac{(y-\mu_Q)^2+\sigma_Q^2}{2\sigma^2}
-\frac12\left[
\log\frac{\tau^2}{\sigma_Q^2}
+\frac{\sigma_Q^2+\mu_Q^2}{\tau^2}-1
\right].
$$

Differentiation gives

$$
\mu_Q^*=\frac{\tau^2}{\sigma^2+\tau^2}y=\widetilde\theta,
\qquad
(\sigma_Q^2)^*=\frac{\sigma^2\tau^2}{\sigma^2+\tau^2}=\sigma_\theta^2.
$$

The Gaussian variational family contains the exact posterior, so its best member is the posterior itself and the maximized ELBO equals $\log Z$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 219](../../../../paper-219-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
