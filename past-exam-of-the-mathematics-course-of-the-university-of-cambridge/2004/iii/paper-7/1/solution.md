<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [harmonic function](../../../../../harmonic-function.md) on $\Omega$ is a twice continuously differentiable function satisfying $\Delta u=0$ there. For complex-valued functions this means that both its [real part](../../../../../real-part.md) and its [imaginary part](../../../../../imaginary-part.md) are [harmonic functions](../../../../../harmonic-function.md). The [mean value property for harmonic functions](../../../../../mean-value-property-for-harmonic-functions.md) characterizes harmonicity: a [continuous function](../../../../../continuous-function.md) is harmonic exactly when its value at each point equals its average over every [sphere](../../../../../sphere.md), or equivalently every ball, whose closed ball lies in $\Omega$. In the forward direction, the derivative of the spherical average vanishes by the [divergence theorem](../../../../../divergence-theorem.md). Conversely, radial smoothing leaves a [continuous function](../../../../../continuous-function.md) with the mean value property unchanged locally; it is therefore smooth. Expanding its small-ball average gives $u(x)+r^2\Delta u(x)/(2(d+3))+o(r^2)$ in dimension $d+1$, and hence $\Delta u=0$.

Write $M=\|u\|_{h^1}$ and $v_{d+1}$ for the volume of the unit ball in $\mathbb R^{d+1}$. We first obtain a pointwise estimate directly from the [mean value property for harmonic functions](../../../../../mean-value-property-for-harmonic-functions.md), before using any boundary representation. For the ball of radius $r=t/2$ centered at $(x,t)$,

$$
|u(x,t)|\leq\frac{1}{v_{d+1}r^{d+1}}\int_{t-r}^{t+r}\int_{\mathbb R^d}|u(y,s)|\,dy\,ds
\leq\frac{2^{d+1}}{v_{d+1}}\frac{M}{t^d}.
$$

Thus every upward shift of $u$ is a bounded [harmonic function](../../../../../harmonic-function.md), with a continuous bounded boundary value.

The required map is the [Poisson integral](../../../../../poisson-integral.md)

$$
P\mu(x,t)=\int_{\mathbb R^d}P_t(x-y)\,d\mu(y),\qquad
P_t(x)=c_d\frac{t}{(t^2+|x|^2)^{(d+1)/2}},\qquad
c_d=\frac{\Gamma((d+1)/2)}{\pi^{(d+1)/2}}.
$$

The [Poisson kernel for the upper half-space](../../../../../poisson-kernel-for-the-upper-half-space.md) is positive, has integral one, and is harmonic as a function of $(x,t)$. Its normalization follows by polar coordinates and $r=\tan\theta$, which reduces the radial integral to $\int_0^{\pi/2}\sin^{d-1}\theta\,d\theta$; direct differentiation gives $\Delta_{x,t}P_t=0$. Differentiation under the integral on compact subsets proves that $P\mu$ is a [harmonic function](../../../../../harmonic-function.md). [Tonelli theorem](../../../../../tonelli-theorem.md) gives

$$
\int|P\mu(x,t)|\,dx\leq\int\int P_t(x-y)\,dx\,d|\mu|(y)=\|\mu\|_{\mathrm{TV}}.
$$

Here the [total variation norm of a measure](../../../../../total-variation-norm-of-a-measure.md) is the [norm](../../../../../norm.md) on finite signed or complex [Borel measures](../../../../../borel-measure.md).

The [Poisson kernel for the upper half-space](../../../../../poisson-kernel-for-the-upper-half-space.md) is an [approximate identity](../../../../../approximate-identity.md): for $\psi\in C_0(\mathbb R^d)$, $P_t*\psi\to\psi$ uniformly. Indeed, [uniform continuity](../../../../../uniform-continuity.md) controls translations smaller than a fixed radius, and the kernel mass outside that radius tends to zero. Consequently

$$
\int\psi(x)P\mu(x,t)\,dx\longrightarrow\int\psi\,d\mu.
$$

The dual characterization of the [total variation norm of a measure](../../../../../total-variation-norm-of-a-measure.md), as the supremum over $\psi\in C_0$ of supremum [norm](../../../../../norm.md) at most one, now gives the reverse inequality $\|\mu\|_{\mathrm{TV}}\leq\|P\mu\|_{h^1}$. Thus $P$ is a linear [isometry](../../../../../isometry.md) and is injective.

For surjectivity, fix $s>0$ and put $u_s(x)=u(x,s)$. Bounded harmonic uniqueness in the upper half-space gives

$$
u(x,s+t)=P_t*u_s(x),\qquad t>0.
$$

To justify this uniqueness, subtract the [Poisson integral](../../../../../poisson-integral.md) of the bounded continuous boundary value from the upward-shifted harmonic function. Their difference is bounded and harmonic and has zero continuous boundary values. Its odd reflection across the boundary is an entire bounded [harmonic function](../../../../../harmonic-function.md); the reflection is harmonic across the flat boundary by [harmonic odd reflection across a hyperplane](../../../../../harmonic-odd-reflection-across-a-hyperplane.md). The [Liouville theorem for harmonic functions](../../../../../harmonic-liouville-theorem.md) makes it constant, and oddness makes it zero. The initial pointwise estimate supplies the boundedness needed here. To see the reflection locally, take a ball centered on the hyperplane and extend the boundary data on its upper hemisphere oddly to its lower hemisphere. The harmonic solution on this ball is odd and zero on its equatorial disk. The [maximum principle for harmonic functions](../../../../../maximum-principle-for-harmonic-functions.md) identifies it with the given difference on the upper half-ball, proving that the reflected function is harmonic across the boundary.

Choose $s_j\downarrow0$. The measures $u_{s_j}\,dx$ have [total variation norm of a measure](../../../../../total-variation-norm-of-a-measure.md) at most $M$. By the [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md), and separability of $C_0(\mathbb R^d)$, a [subsequence](../../../../../subsequence.md) converges in the [weak-star topology](../../../../../weak-star-topology.md) to a finite measure $\mu$ with $\|\mu\|_{\mathrm{TV}}\leq M$. For fixed $(x,t)$ and $s_j<t$,

$$
u(x,t)=\int P_{t-s_j}(x-y)u(y,s_j)\,dy.
$$

The kernels in this display belong to $C_0$ and converge uniformly to $P_t(x-\cdot)$. The uniform measure [norm](../../../../../norm.md) bound therefore allows passage to the limit, giving $u(x,t)=P\mu(x,t)$. This proves the [Poisson representation of harmonic h1 by finite measures](../../../../../poisson-representation-of-harmonic-h1-by-finite-measures.md), including onto-ness.

Finally $P_t(x)\leq c_dt^{-d}$, so the [Poisson representation of harmonic h1 by finite measures](../../../../../poisson-representation-of-harmonic-h1-by-finite-measures.md) improves the preliminary pointwise constant:

$$
\boxed{\|P\mu\|_{h^1}=\|\mu\|_{\mathrm{TV}},\qquad |u(x,t)|\leq c_dt^{-d}\|u\|_{h^1}.}
$$

The last occurrence of $h^1(\mathbb R^{d+1})$ in the printed question is understood as the [harmonic Hardy space of the upper half-space](../../../../../harmonic-hardy-space-of-the-upper-half-space.md) defined earlier in that question.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
