<h1 id="26k/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Here $\alpha>0$ and $\gamma_j>0$. The asset payoff has a centered [Laplace distribution](../../../../../../laplace-distribution.md). Its [moment-generating function](../../../../../../moment-generating-function.md) is $\mathbb E e^{tX}=\alpha^2/(\alpha^2-t^2)$ for $|t|<\alpha$, and diverges otherwise. Expected [constant absolute risk aversion utility](../../../../../../constant-absolute-risk-aversion-utility.md) for a holding $\theta$ is

$$
-e^{-\gamma_jw_0}\,e^{\gamma_jp\theta}\frac{\alpha^2}{\alpha^2-\gamma_j^2\theta^2}.
$$

To maximize it, minimize the logarithm of the positive factor on $|\gamma_j\theta|<\alpha$. Its derivative is $\gamma_jp+2\gamma_j^2\theta/(\alpha^2-\gamma_j^2\theta^2)$, and its second derivative is strictly positive. It diverges at the endpoints, so the unique critical point is the global optimizer:

$$
\boxed{\theta_j=-\frac{\sqrt{1+p^2\alpha^2}-1}{\gamma_jp}.}
$$

At $p=0$ use the continuous limit $\theta_j=0$. The other quadratic root is outside the finite-utility domain.

Let $\Gamma^{-1}=\sum_j\gamma_j^{-1}$. Aggregate demand is $D(p)=-(\sqrt{1+p^2\alpha^2}-1)/(\Gamma p)$. Unit positive supply requires $p<0$ and $\sqrt{1+p^2\alpha^2}=1-\Gamma p$. Squaring and excluding $p=0$ gives

$$
\boxed{p=-\frac{2\Gamma}{\alpha^2-\Gamma^2}\quad(\alpha>\Gamma).}
$$

This negative price satisfies the unsquared equation and every individual finite-utility constraint. When $\alpha\leq\Gamma$, there is **no finite clearing price**. Indeed $D(p)<\alpha/\Gamma$ for every finite negative $p$, with limit $\alpha/\Gamma$ as $p\to-\infty$. If $\alpha<\Gamma$ this maximum limiting demand is below supply; if equal, demand only approaches one at an infinitely negative price. A formal positive solution obtained by squaring when $\alpha<\Gamma$ violates the original demand equation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [26K](../../26k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
