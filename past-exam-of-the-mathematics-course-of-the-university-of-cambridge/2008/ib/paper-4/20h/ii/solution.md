<h1 id="20h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Capital and labour are nonnegative inputs. On the budget line, $0\leq K\leq b$ and $L=(b-K)/w$. Both endpoints give zero output, whereas every interior point has positive output, so the maximum is interior. The [Lagrangian](../../../../../../lagrangian.md) with the sign convention of part (i) is

$$
\mathcal L(K,L,\lambda)=K^\alpha L^\beta+\lambda(b-K-wL).
$$

Its stationarity equations are $\alpha K^{\alpha-1}L^\beta=\lambda$ and $\beta K^\alpha L^{\beta-1}=w\lambda$. Dividing by the positive output gives $\alpha/K=\lambda/f$ and $\beta/L=w\lambda/f$, hence $wL=(\beta/\alpha)K$. Together with the budget constraint this yields

$$
\boxed{K_* =\frac{\alpha b}{\alpha+\beta},\qquad L_* =\frac{\beta b}{w(\alpha+\beta)}.}
$$

To verify the unique global maximum, maximize the logarithm of the [Cobb–Douglas production function](../../../../../../cobb-douglas-production-function.md) along the budget line:

$$
\log f=\alpha\log K+\beta\log(b-K)-\beta\log w,\qquad\frac{d^2}{dK^2}\log f=-\frac\alpha{K^2}-\frac\beta{(b-K)^2}<0.
$$

Its unique stationary point is therefore the unique maximum, including comparison with the zero-output boundary points.

Writing $r=\alpha+\beta$ and $C=(\alpha/r)^\alpha(\beta/(wr))^\beta$, the optimal output is $\phi(b)=Cb^r$. The [Lagrange multiplier](../../../../../../lagrange-multiplier.md) obtained from the first stationarity equation is $\lambda=\alpha\phi/K_*=r\phi/b$. Direct differentiation verifies the [envelope theorem](../../../../../../envelope-theorem.md) identity:

$$
\boxed{\phi(b)=\left(\frac\alpha{\alpha+\beta}\right)^\alpha\left(\frac\beta{w(\alpha+\beta)}\right)^\beta b^{\alpha+\beta},\qquad\phi'(b)=\lambda(b)=\frac{(\alpha+\beta)\phi(b)}b.}
$$

For clarity, the global dual-supremum premise of part (i) need not hold for every exponent pair allowed here. If $r>1$, along $(K,L)=(tK_*,tL_*)$ the unrestricted [Lagrangian](../../../../../../lagrangian.md) is $t^r\phi(b)+\lambda b(1-t)$, which tends to infinity for every finite $\lambda$. Thus the verification above is by constrained stationarity and direct differentiation, and remains valid even when that stronger global [Lagrangian duality](../../../../../../lagrangian-duality.md) representation fails.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [20H](../../20h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
