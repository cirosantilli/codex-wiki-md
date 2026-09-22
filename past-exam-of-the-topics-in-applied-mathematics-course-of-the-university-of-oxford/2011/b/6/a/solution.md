<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For uniform nearest-neighbor bonds of strength $K_0$ on a ring with $N\geq3$, retain the normalization of the given model:

$$
\boxed{\dot\theta_i=\omega_i+\frac{K_0}{N}\bigl[\sin(\theta_{i-1}-\theta_i)+\sin(\theta_{i+1}-\theta_i)\bigr],}
$$

with indices interpreted modulo $N$. On an open chain the interior equations are the same, while

$$
\dot\theta_1=\omega_1+\frac{K_0}{N}\sin(\theta_2-\theta_1),\qquad\dot\theta_N=\omega_N+\frac{K_0}{N}\sin(\theta_{N-1}-\theta_N).
$$

For nonuniform bonds, replace each $K_0$ by the corresponding $K_{ij}$. A convention without the factor $1/N$ is obtained by rescaling the bond strengths; it is not silently substituted here.

For all-to-all coupling define the [Kuramoto order parameter](../../../../../kuramoto-order-parameter.md)

$$
\boxed{re^{i\psi}=\frac1N\sum_{j=1}^Ne^{i\theta_j}.}
$$

It is the centroid of unit phase vectors: $r$ measures phase coherence and $\psi$ the mean phase. Multiplying by $e^{-i\theta_i}$ and taking imaginary parts gives

$$
\boxed{\dot\theta_i=\omega_i+Kr\sin(\psi-\theta_i).}
$$

Thus only the two components of the [Kuramoto order parameter](../../../../../kuramoto-order-parameter.md) mediate interaction.

For the symmetric stationary continuum branch, choose the rotating frame with $\psi=0$. Oscillators with $|\omega|\leq Kr$ lock at $\theta=\arcsin(\omega/(Kr))$, choosing $\cos\theta>0$ for stability. Those with $|\omega|>Kr$ drift, with stationary phase density proportional to $|\omega-Kr\sin\theta|^{-1}$. Their real contribution to the order parameter vanishes, since the integral of $\cos\theta/(\omega-Kr\sin\theta)$ over a period is the change of a periodic logarithm. Their imaginary contributions cancel between $\omega$ and $-\omega$ because $g$ is symmetric.

The locked oscillators therefore give the real self-consistency relation

$$
r=\int_{-Kr}^{Kr}\sqrt{1-\frac{\omega^2}{K^2r^2}}\,g(\omega)\,d\omega.
$$

Set $\omega=Kr\sin\theta$ and divide by $r>0$ to obtain

$$
\boxed{1=K\int_{-\pi/2}^{\pi/2}\cos^2\theta\,g(Kr\sin\theta)\,d\theta.}
$$

This is the [Kuramoto self-consistency equation](../../../../../kuramoto-self-consistency-equation.md) for partial synchronization. The incoherent state $r=0$ must be considered before this division. If $g$ is continuous at zero with $0<g(0)<\infty$, the branch meets incoherence at $K_c=2/[\pi g(0)]$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../split.md)
6. [Topics in applied mathematics course of the University of Oxford](../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
