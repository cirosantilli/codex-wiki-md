<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [tautological bundle](../../../../../tautological-bundle.md) over [Complex projective space](../../../../../complex-projective-space.md) is

$$
\mathcal O(-1)=\{([z],v)\in\mathbb {CP}^n\times\mathbb C^{n+1}:v\in\mathbb Cz\}.
$$

On $U_i=\{z_i\ne0\}$, the vector $e_i([z])=z/z_i$ is a holomorphic frame. On $U_i\cap U_j$,

$$
e_j=\frac{z_i}{z_j}e_i,
$$

so the transition functions are holomorphic. Define $\mathcal O(1)=\mathcal O(-1)^*$ and, for $k\in\mathbb Z$, define $\mathcal O(k)=\mathcal O(1)^{\otimes k}$ when $k\geq0$ and $\mathcal O(k)=\mathcal O(-1)^{\otimes(-k)}$ when $k<0$. Its transition functions are the corresponding $k$th powers of those of $\mathcal O(1)$, equivalently the $(-k)$th powers of those of $\mathcal O(-1)$.

A nonzero linear functional $\ell\in(\mathbb C^{n+1})^*$ restricts on each projective line to define a global [holomorphic section](../../../../../holomorphic-section.md) $s_\ell$ of $\mathcal O(1)$. Its zero divisor is the [projective hyperplane](../../../../../projective-hyperplane.md) $H_\ell=\{[z]:\ell(z)=0\}$, so every hyperplane is an effective divisor of $\mathcal O(1)$.

Conversely, let $D$ be the divisor of a nonzero section of $\mathcal O(1)$. In the affine chart $z_0=1$, the section is represented by an entire function $f$ on $\mathbb C^n$. Compatibility with the other projective charts gives the linear growth bound in the question along every complex affine line. The supplied Liouville-type result makes $f$ affine-linear, and homogenizing it gives a linear functional $\ell$ on $\mathbb C^{n+1}$. Thus $D=H_\ell$.

In local coordinates centred at $x$, the [blowup of a complex manifold at a point](../../../../../blowup-of-a-complex-manifold-at-a-point.md) is modeled by

$$
\widetilde{mathbb C^n}
=\{(z,[v])\in\mathbb C^n\times\mathbb {CP}^{n-1}:z\in\mathbb Cv\},
\qquad \sigma(z,[v])=z.
$$

On the chart $v_i\ne0$, write $u=z_i$ and $t_j=v_j/v_i$; then $z_j=ut_j$, giving holomorphic coordinates $(u,(t_j)_{j\ne i})$. These charts show that the blowup is a complex manifold, that $\sigma$ is holomorphic, and that its exceptional fiber is $\mathbb {CP}^{n-1}$. A biholomorphic coordinate change at the centre lifts by sending a punctured point together with its limiting tangent direction to its image; the chart formulas extend across the exceptional divisor. Hence the construction is independent of coordinates up to biholomorphism.

For $a(z)=-z$ on $\mathbb C^2$, define

$$
\widetilde a(z,[v])=(-z,[v]).
$$

This is holomorphic and satisfies $\sigma\circ\widetilde a=a\circ\sigma$. The blowup $\widetilde{mathbb C^2}$ is the total space of $\mathcal O(-1)\to\mathbb {CP}^1$, and $\widetilde a$ acts as multiplication by $-1$ in every fiber. The invariant fiber coordinate is $w=u^2$. If $u_j=g_{ji}u_i$ are the transition laws for $\mathcal O(-1)$, then $w_j=g_{ji}^2w_i$, which are the transition laws for $\mathcal O(-2)$. Thus the local quotient maps $(t,u)\mapsto(t,u^2)$ glue, give the quotient a complex-manifold atlas even along the fixed zero section, and yield

$$
\boxed{\widetilde{mathbb C^2}/\langle\widetilde a\rangle\cong\operatorname{Tot}\mathcal O(-2).}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 118](../../paper-118-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
