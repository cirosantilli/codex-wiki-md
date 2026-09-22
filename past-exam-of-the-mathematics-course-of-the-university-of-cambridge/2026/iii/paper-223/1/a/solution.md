<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [gross-error sensitivity](../../../../../../gross-error-sensitivity.md) is $\gamma^*(T,F)=\sup_x|\operatorname{IF}(x;T,F)|$. At $N(\theta,1)$, the [influence function of the sample median](../../../../../../influence-function-of-the-sample-median.md) has magnitude $1/(2\varphi(0))=\sqrt{\pi/2}$, so

$$
\gamma^*(\widehat\theta_{\mathrm{med}})=\sqrt{\frac\pi2}.
$$

For the [Huber location estimator](../../../../../../huber-location-estimator.md), $\psi_k(u)=\max(-k,\min(u,k))$ and $\mathbb E\psi_k'(Z)=\mathbb P(|Z|\leq k)=2\Phi(k)-1$, giving

$$
\gamma^*(\widehat\theta_{\mathrm{Hub},k})
=\frac{k}{2\Phi(k)-1}.
$$

For the symmetric normal law, the trimmed population mean is $\theta$. Writing $q_\gamma=\Phi^{-1}(1-\gamma)$ in the supplied influence function gives

$$
\boxed{\gamma^*(\widehat\theta_{\mathrm{trim},\gamma})
=\frac{q_\gamma}{1-2\gamma}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
