<h1 id="40e/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the high-frequency indices $(n+1)/2\leq k\leq n$, the angle $\theta_k=k\pi/(n+1)$ ranges from $\pi/2$ to $\pi-\pi/(n+1)$. Since

$$
\lambda_k(\omega)=1-\omega+\omega\cos\theta_k,
$$

the large-$n$ [high-frequency smoothing factor of weighted Jacobi](../../../../../../high-frequency-smoothing-factor-of-weighted-jacobi.md) is

$$
\boxed{
\mu_\omega
=\max_{\pi/2\leq\theta\leq\pi}
|1-\omega+\omega\cos\theta|
=\max\{|1-\omega|,|1-2\omega|\}.}
$$

For $0<\omega<1$, this is strictly less than one independently of $n$, so high-frequency error decays geometrically much faster than the low-frequency factor $1-O(n^{-2})$.

To minimize $\mu_\omega$, balance the endpoint magnitudes:

$$
1-\omega=2\omega-1.
$$

Thus the optimal relaxation and attenuation factors are

$$
\boxed{\omega_*=\frac23,
\qquad
\mu_*=\frac13.}
$$

For finite $n$, retaining the endpoint $\cos(\pi-\pi/(n+1))=-\cos(\pi/(n+1))$ gives

$$
\omega_*=\frac{2}{2+\cos(\pi/(n+1))},
\qquad
\mu_*=\frac{\cos(\pi/(n+1))}
{2+\cos(\pi/(n+1))},
$$

which tend to $2/3$ and $1/3$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [40E](../../40e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
