<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

At the [standard normal distribution](../../../../../../standard-normal-distribution.md), symmetry and the odd [Huber score](../../../../../../huber-score.md) give population root zero. For $0<b<\infty$, the derivative of the clipped score is $\mathbf1_{\{|x|<b\}}$ except at its two corners, which have zero normal probability. Put $m_b=2\Phi(b)-1>0$ and write $\phi$ for the [standard normal density](../../../../../../standard-normal-density.md). The [sandwich variance of an M-estimator](../../../../../../sandwich-variance-of-an-m-estimator.md) has numerator

$$
\mathbb E\psi_b(Z)^2=\int_{-b}^b z^2\phi(z)dz+2b^2[1-\Phi(b)].
$$

Using $\phi'(z)=-z\phi(z)$ and integration by parts,

$$
\int_{-b}^b z^2\phi(z)dz=-2b\phi(b)+2\Phi(b)-1.
$$

Therefore

$$
\boxed{V(\psi_b,\Phi)=\frac{2\Phi(b)-1-2b\phi(b)+2b^2[1-\Phi(b)]}{[2\Phi(b)-1]^2}.}
$$

As checks, it tends to $1$ as $b\to\infty$, the [sample mean](../../../../../../sample-mean.md) limit, and to $\pi/2$ as $b\downarrow0$, the [sample median](../../../../../../sample-median.md) limiting [variance](../../../../../../variance-split.md). The estimator [variance](../../../../../../variance-split.md) for a sample of size $n$ is approximately this quantity divided by $n$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
