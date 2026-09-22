<h1 id="6h/solution">Solution</h1>

↑ **Parent:** [6H](../6h.md)

The Neyman–Pearson lemma says that among tests of size at most $\alpha$ for two simple hypotheses, a [likelihood-ratio test](../../../../../likelihood-ratio-test.md) rejecting where $p(x;\theta_1)/p(x;\theta_0)>k$ is most powerful, with boundary randomisation if required. If $\varphi$ is that test and $\psi$ any competing test, choose $k$ so the sizes agree. Pointwise,

$$
(\varphi-\psi)(p_1-kp_0)\ge0.
$$

Integration and the size inequality yield $E_1\varphi\ge E_1\psi$.

Here

$$
\frac{p(x;\theta_1)}{p(x;\theta_0)}=\frac{\theta_1}{\theta_0}e^{-(\theta_1-\theta_0)|x|},
$$

which decreases with $|x|$. Thus reject for $|X|\le c$, where

$$
\boxed{\alpha=P_{\theta_0}(|X|\le c)=1-e^{-\theta_0c},\qquad
c=-\frac1{\theta_0}\log(1-\alpha).}
$$

## ↑ Ancestors (10)

1. [6H](../6h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
