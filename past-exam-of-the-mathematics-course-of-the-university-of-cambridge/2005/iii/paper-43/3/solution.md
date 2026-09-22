<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For the [Poisson process](../../../../../poisson-process.md) of claims and [relative safety loading](../../../../../relative-safety-loading.md) $\rho$, the premium rate in the [classical risk model](../../../../../classical-risk-model.md) is $c=(1+\rho)\lambda\mu$. Dividing the [adjustment coefficient](../../../../../adjustment-coefficient.md) equation $\lambda(M(r)-1)=cr$ by $\lambda$ explains why the arrival rate cancels. Interpret $r_\infty$ as the upper endpoint of the finite [moment-generating function](../../../../../moment-generating-function.md) domain, so $M(r)<\infty$ for $0\leq r<r_\infty$ and its stated divergence occurs at that endpoint.

Set $F(r)=M(r)-1-(1+\rho)\mu r$. Then

$$
F(0)=0,\qquad F'(0)=-\rho\mu<0,\qquad
F''(r)=\mathbb E[X_1^2e^{rX_1}]>0\quad(0\leq r<r_\infty).
$$

Differentiation is valid inside the finite-transform domain, and its positive neighbourhood gives finite [moments](../../../../../moment.md) of every order. Thus $F$ is [strictly convex](../../../../../strictly-convex-function.md) and negative just to the right of zero. If $r_\infty<\infty$, divergence of $M(r)$ makes $F(r)\to\infty$ at the endpoint. If $r_\infty=\infty$, choose $a>0$ with $\mathbb P(X_1\geq a)>0$; then $M(r)\geq\mathbb P(X_1\geq a)e^{ar}$, which eventually exceeds every [linear function](../../../../../linear-function.md). Again $F(r)\to\infty$. The [intermediate value theorem](../../../../../intermediate-value-theorem.md) gives a positive zero.

There is at most one positive zero: [strict convexity](../../../../../strictly-convex-function.md) and $F(0)=0$ make the secant slope $F(r)/r$ strictly increasing for $r>0$. It starts at $-\rho\mu$ and crosses zero exactly once. Hence

$$
\boxed{\text{There is a unique }R\in(0,r_\infty)\text{ with }M(R)-1=(1+\rho)\mu R.}
$$

This proves the [secant-slope existence criterion for an adjustment coefficient](../../../../../secant-slope-existence-criterion-for-an-adjustment-coefficient.md) in the present setting.

Put $m_j=\mathbb EX_1^j$. For $u>0$, the positive remainder of the [exponential series](../../../../../exponential-series.md) gives $e^u>1+u+u^2/2$. Apply it to $u=RX_1$ and take [expectations](../../../../../expected-value.md):

$$
(1+\rho)\mu R=M(R)-1>\mu R+\frac{m_2R^2}{2}.
$$

Dividing by $R>0$ yields

$$
\boxed{R<r_1=\frac{2\rho\mu}{m_2}.}
$$

Keeping the cubic term similarly gives

$$
\rho\mu>\frac{m_2R}{2}+\frac{m_3R^2}{6}.
$$

The [polynomial](../../../../../polynomial-split.md) $g(r)=m_3r^2+3m_2r-6\rho\mu$ is strictly increasing for $r\geq0$, is negative at zero and tends to infinity. Let $r_2$ be its unique positive zero. The last inequality says $g(R)<0$, so

$$
\boxed{R<r_2=\frac{\sqrt{9m_2^2+24\rho\mu m_3}-3m_2}{2m_3},\qquad
g(r_2)=0.}
$$

Finally, $3m_2r_1=6\rho\mu$, whence $g(r_1)=m_3r_1^2>0$. Monotonicity gives $r_2<r_1$. Thus the requested [upper bounds](../../../../../upper-bound-in-a-partially-ordered-set.md) can in fact be sharpened to the strict ordering **$0<R<r_2<r_1$**. The bounds themselves need not lie in the finite-transform domain; the argument only evaluates the actual transform at $R$ and [polynomial](../../../../../polynomial-split.md) [moments](../../../../../moment.md) elsewhere. These are [polynomial moment bounds for the adjustment coefficient](../../../../../polynomial-moment-bounds-for-the-adjustment-coefficient.md).

For rate-$\alpha$ [exponential distribution](../../../../../exponential-distribution.md) claims,

$$
\mu=\frac1\alpha,\qquad m_2=\frac2{\alpha^2},\qquad m_3=\frac6{\alpha^3},\qquad
M(r)=\frac\alpha{\alpha-r}\quad(r<\alpha).
$$

The positive root satisfies $1/(\alpha-R)=(1+\rho)/\alpha$ after dividing out $R$, so

$$
\boxed{R=\frac{\alpha\rho}{1+\rho},\qquad
r_1=\alpha\rho,\qquad
r_2=\frac\alpha2\left(\sqrt{1+4\rho}-1\right).}
$$

The cubic-bound equation reduces to $r_2^2+\alpha r_2-\rho\alpha^2=0$, selecting the displayed positive root. In particular $R<\alpha$, as required by the transform domain, for every $\rho>0$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
