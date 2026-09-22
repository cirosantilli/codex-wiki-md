<h1 id="19d/solution">Solution</h1>

↑ **Parent:** [19D](../19d.md)

Repeated [integration by parts](../../../../../integration-by-parts.md) in

$$
\frac1{k!}\int_a^x(x-\theta)^kf^{(k+1)}(\theta)\,d\theta
$$

produces the first $k+1$ terms of the [Taylor polynomial](../../../../../taylor-polynomial.md) and leaves $f(x)$, proving the [integral remainder in Taylor theorem](../../../../../integral-remainder-in-taylor-theorem.md)

$$
R(x)=\frac1{k!}\int_a^x(x-\theta)^kf^{(k+1)}(\theta)\,d\theta.
$$

Apply the linear functional $\lambda_k$ to this identity. It annihilates the Taylor polynomial, and commuting it with integration gives the [Peano kernel theorem](../../../../../peano-kernel-theorem.md)

$$
\lambda_k[f]=\frac1{k!}\int_a^b\lambda_k[(x-\theta)^+_k]f^{(k+1)}(\theta)\,d\theta.
$$

For the [midpoint quadrature rule](../../../../../midpoint-quadrature-rule.md) on $[0,1]$, $e[1]=e[x]=0$, so $k=1$. Its [Peano kernel](../../../../../peano-kernel.md) is

$$
K(\theta)=\int_0^1(x-\theta)_+\,dx-(1/2-\theta)_+
=\begin{cases}
\theta^2/2,&0\leq\theta\leq1/2,\\
(1-\theta)^2/2,&1/2\leq\theta\leq1.
\end{cases}
$$

For $f(x)=x^2$, the formula gives

$$
e[f]=\int_0^1K(\theta)f''(\theta)\,d\theta=2\int_0^1K(\theta)\,d\theta=\frac1{12},
$$

agreeing with $\int_0^1x^2dx-(1/2)^2=1/3-1/4$.

## ↑ Ancestors (10)

1. [19D](../19d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
