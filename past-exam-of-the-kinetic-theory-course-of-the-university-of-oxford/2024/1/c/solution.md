<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For fixed $\mathbf R$ and $t$, define $h(\mathbf x,s)=n_2(\mathbf a,\mathbf b,t)$ with $\mathbf a=\mathbf x+(s-1)\mathbf R$ and $\mathbf b=\mathbf x+s\mathbf R$. The [chain rule](../../../../chain-rule.md) gives

$$
\partial_sh=\mathbf R\cdot(\nabla_{\mathbf a}+\nabla_{\mathbf b})n_2,\qquad \nabla_{\mathbf x}h=(\nabla_{\mathbf a}+\nabla_{\mathbf b})n_2,
$$

so $\boxed{\partial_sh=\mathbf R\cdot\nabla_{\mathbf x}h}$. The derivative with respect to $\mathbf x$ here translates _both_ arguments of the [two-particle number density](../../../../two-particle-number-density.md); it is not a derivative of its first argument alone.

Take the spatial divergence of the proposed [interaction pressure tensor](../../../../interaction-pressure-tensor.md). Its [pair potential](../../../../pair-potential.md) factor is independent of $\mathbf x$, so the preceding identity gives

$$
\begin{aligned}
\partial_{x_j}P^\phi_{ij}
&=-\frac12\int d^3R\,\frac{R_i\phi'(R)}R\int_0^1\partial_sh\,ds\\
&=-\frac12\int d^3R\,\frac{R_i\phi'(R)}R\left[n_2(\mathbf x,\mathbf x+\mathbf R)-n_2(\mathbf x-\mathbf R,\mathbf x)\right].
\end{aligned}
$$

Exchange symmetry of the [two-particle distribution function](../../../../two-particle-distribution-function.md) implies $n_2(\mathbf x-\mathbf R,\mathbf x)=n_2(\mathbf x,\mathbf x-\mathbf R)$. In the second term, substitute $\mathbf R\mapsto-\mathbf R$. Since $R_i\phi'(R)/R$ is odd, both terms become equal:

$$
\partial_{x_j}P^\phi_{ij}=-\int d^3R\,\frac{R_i\phi'(R)}R\,n_2(\mathbf x,\mathbf x+\mathbf R).
$$

On the other hand, at fixed $\mathbf x_\star=\mathbf x+\mathbf R$, the first-argument derivative of the [pair potential](../../../../pair-potential.md) is $\nabla_{\mathbf x}\phi=-\mathbf R\phi'(R)/R$. Thus the interaction [force density](../../../../force-density.md) in [b](../b.md) is $-\partial_{x_j}P^\phi_{ij}$. Moving it to the left yields local [conservation of momentum](../../../../momentum-conservation.md):

$$
\boxed{\partial_t(\rho\mathbf u)+\nabla\cdot(\rho\mathbf u\mathbf u+\mathbf P+\mathbf P^\phi)=0.}
$$

The integral over $s$ distributes each pair's [momentum flux](../../../../momentum-flux.md) along the straight segment joining the particles. The factor $1/2$ removes the double counting of ordered pairs. Central [forces](../../../../force-split.md) also make $P^\phi_{ij}=P^\phi_{ji}$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
