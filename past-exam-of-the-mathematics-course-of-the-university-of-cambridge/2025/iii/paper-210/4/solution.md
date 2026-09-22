<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

With densities $p,q$,

$$
\operatorname{TV}(P,Q)=\frac12\int|p-q|d\mu,
\qquad
H(P,Q)^2=\int(\sqrt p-\sqrt q)^2d\mu.
$$

By [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md),

$$
\operatorname{TV}(P,Q)
\leq\frac12H(P,Q)
\left(\int(\sqrt p+\sqrt q)^2d\mu\right)^{1/2}
\leq H(P,Q).
$$

Also $(\sqrt p-\sqrt q)^2\leq|p-q|$, so $H^2\leq2\operatorname{TV}$.

The Hellinger affinity is $\rho(P,Q)=\int\sqrt{pq}\,d\mu=1-H^2/2$. Product densities and [Fubini's theorem](../../../../../fubini-s-theorem.md) give $\rho(P^n,Q^n)=\rho(P,Q)^n$, hence

$$
H^2(P^n,Q^n)=2-2\left(1-\frac12H^2(P,Q)\right)^n.
$$

[Le Cam two-point lemma](../../../../../le-cam-two-point-lemma.md) states, for squared-error estimation at parameter points $\theta_0,\theta_1$, that

$$
\inf_{\widehat\theta}\max_{j=0,1}
\mathbb E_j(\widehat\theta-\theta_j)^2
\geq\frac{(\theta_1-\theta_0)^2}{8}
\left(1-\operatorname{TV}(P_0,P_1)\right).
$$

Take $\theta_0=0$, $\theta_1=\delta=1/(4n)$. The one-observation uniform densities overlap on length $1-\delta$, so $H^2(P_0,P_1)=2\delta$. Therefore

$$
H^2(P_0^n,P_1^n)
=2-2(1-\delta)^n\leq2n\delta=\frac12.
$$

The first distance inequality gives $\operatorname{TV}(P_0^n,P_1^n)\leq1/\sqrt2$. Le Cam's lemma now yields

$$
\inf_{\widehat\theta}\sup_{\theta\in\mathbb R}
\mathbb E_\theta(\widehat\theta-\theta)^2
\geq\frac{1-1/\sqrt2}{128n^2}.
$$

This proves the claim with the displayed universal positive constant.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
