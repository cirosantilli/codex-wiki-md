<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Fourier transform](../../../../../../fourier-transform.md) on the infinite spatial lattice gives

$$
a_{n+1}=2iA(\theta)a_n+a_{n-1},\qquad
A(\theta)=a_1\sin\theta+a_2\sin2\theta,
$$

with [polynomial roots](../../../../../../root-of-a-polynomial.md) $G_\pm=iA\pm\sqrt{1-A^2}$. When $|A|$ is uniformly less than one, the [polynomial roots](../../../../../../root-of-a-polynomial.md) have modulus one and a uniform positive separation. Diagonalizing the [companion matrix](../../../../../../companion-matrix.md) then bounds all its powers independently of $\theta$ and $n$. [Parseval's identity](../../../../../../parseval-identity.md) proves [stability](../../../../../../stability-of-a-numerical-method.md) in the discrete $L^2$ [norm](../../../../../../norm.md) for arbitrary square-summable starting perturbations at both levels.

At $\mu=1/2$ the coefficients give

$$
A(\theta)=\frac58\sin\theta-\frac1{16}\sin2\theta
=\frac{\sin\theta(5-\cos\theta)}8,\qquad |A(\theta)|\le\frac34<1.
$$

Consequently **$\mu=1/2$ is stable**.

At $\mu=3/2$,

$$
A(\theta)=\frac78\sin\theta+\frac5{16}\sin2\theta,
\qquad A(\pi/3)=\frac{19\sqrt3}{32}>1.
$$

The growing [polynomial root](../../../../../../root-of-a-polynomial.md) at this phase has modulus

$$
\boxed{|G|=\frac{19\sqrt3+\sqrt{59}}{32}>1.}
$$

To turn this into a [Cauchy problem](../../../../../../cauchy-problem.md) [linear instability](../../../../../../linear-instability.md) proof, rather than rely on a [plane wave](../../../../../../plane-wave.md) of infinite [norm](../../../../../../norm.md), choose a small interval around $\pi/3$ on which the growing [polynomial root](../../../../../../root-of-a-polynomial.md) has modulus at least $1+\delta$. Choose an initial [Fourier transform](../../../../../../fourier-transform.md) amplitude that is a nonzero [square-integrable function](../../../../../../square-integrable-function.md) supported there, and set the level-one amplitude equal to that [polynomial root](../../../../../../root-of-a-polynomial.md) times the level-zero amplitude. The recurrence then multiplies by the same growing [polynomial root](../../../../../../root-of-a-polynomial.md) at every step on the support. [Parseval identity](../../../../../../parseval-identity.md) gives $\|u^n\|_2\ge(1+\delta)^n\|u^0\|_2$, whereas both initial [norms](../../../../../../norm.md) are bounded independently of $h$. Real data can be obtained by adding the conjugate interval around $-\pi/3$. Since $n=T/(\mu h)$ tends to infinity at fixed $T$, **$\mu=3/2$ is unstable**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
