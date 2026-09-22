<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

If $v_T=\mathbb E[operatorname{IF}(X;T,N(\theta_0,1))^2]$, asymptotic normality gives an asymptotically level-$\alpha$ test that rejects when

$$
\widehat\theta_T>\theta_0+z_{1-\alpha}\sqrt{v_T/n}.
$$

For the median, $v_T=\pi/2$. For Huber,

$$
v_T=\frac{\mathbb E[\min(Z^2,k^2)]}{(2\Phi(k)-1)^2}.
$$

For the trimmed mean, with $q=\Phi^{-1}(1-\gamma)$,

$$
v_T=\mathbb E\left[
\frac{\max(-q,\min(Z,q))^2}{(1-2\gamma)^2}
\right].
$$

These tests have bounded influence functions, so a small contamination proportion has bounded first-order effect on their statistics, asymptotic levels, and powers. Their finite-contamination protection is quantified by the breakdown points in part (c).

## ↑ Ancestors (11)

1. [D](../d.md)
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
