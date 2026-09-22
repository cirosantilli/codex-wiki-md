<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $0<\lambda<1$ fixed, the denominator stays away from zero, so [dominated convergence](../../../../../../dominated-convergence-theorem.md) gives

$$
J\sim\int_0^1\frac{dx}{(1-\lambda+\lambda x)^2}=\boxed{\frac1{1-\lambda}}.
$$

This approximation remains appropriate on the left of the transition when $1-\lambda\gg\epsilon$. To resolve the [Lorentzian peak approaching an integration endpoint](../../../../../../lorentzian-peak-approaching-an-integration-endpoint.md), let $\lambda-1=\epsilon\tau$ with bounded $\tau$, and put $x=\epsilon X$. The cosine is $1+O(\epsilon^2X^2)$ in the contributing region. Therefore

$$
J\sim\frac1\epsilon\int_0^\infty\frac{dX}{(\lambda X-\tau)^2+1}
=\boxed{\frac1{\epsilon\lambda}\left[\frac\pi2+\arctan\frac{\lambda-1}{\epsilon}\right]}.
$$

Thus the distinguished transition has width **$|\lambda-1|=O(\epsilon)$**. For large negative $\tau$ this expression matches $1/(1-\lambda)$ to leading order; for large positive $\tau$ it gives the full interior-peak contribution.

For $\lambda>1$ away from the transition, the denominator has a narrow minimum at $x_*=1-1/\lambda$. Set $c_* =\cos(\pi x_*/2)=\sin(\pi/(2\lambda))$ and $x-x_*=(\epsilon c_*/\lambda)s$. The slowly varying cosine may be frozen over the peak and the integration limits extended, giving

$$
J\sim\frac1{\epsilon\lambda c_*}\int_{-\infty}^{\infty}\frac{ds}{1+s^2}
=\boxed{\frac\pi{\epsilon\lambda\sin(\pi/(2\lambda))}}.
$$

The small parameter controlling the left-end truncation near $\lambda=1$ is $\epsilon/(\lambda-1)$, so this formula requires $\lambda-1\gg\epsilon$ there.

For $\lambda\gg1$, the peak approaches $x=1$, but its width is $\epsilon\pi/(2\lambda^2)$ whereas its distance from that endpoint is $1/\lambda$. Their ratio is $O(\epsilon/\lambda)$, and the relative variation of the cosine across the peak is also $O(\epsilon/\lambda)$. Hence proximity to the endpoint does not destroy the approximation: the peak becomes narrower still. Equivalently, $s=\lambda(1-x)$ gives $J=\lambda^{-1}\int_0^\lambda[(1-s)^2+\epsilon^2\sin^2(\pi s/(2\lambda))]^{-1}ds$, with its peak at $s=1$. The large-$\lambda$ limit of the leading result is **$J\sim2/\epsilon$**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
