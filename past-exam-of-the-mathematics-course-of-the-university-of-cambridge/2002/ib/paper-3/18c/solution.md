<h1 id="18c/solution">Solution</h1>

↑ **Parent:** [18C](../18c.md)

For steady uniform-density inviscid flow with no body force, the [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md) read $(\mathbf u\cdot\nabla)\mathbf u=-\nabla p/\rho$. Dotting with $\mathbf u$ gives

$$
\mathbf u\cdot\nabla\left(\frac12u^2+\frac p\rho\right)=0.
$$

Thus the [Bernoulli equation](../../../../../bernoulli-equation.md) states that $u^2/2+p/\rho$ is constant along each [streamline](../../../../../streamline.md); the constants need not be the same on unrelated [streamlines](../../../../../streamline.md).

In the slowly varying tube approximation, mass conservation gives $\pi(r-h)^2u=\pi R^2V$, so $r-h=R\sqrt{V/u}$. The upstream Bernoulli constant and the wall [pressure](../../../../../pressure.md) law give

$$
p-p_0=\frac\rho2(V^2-u^2)=k(r-R),\qquad
\frac rR=1+\frac\lambda4\left[1-(u/V)^2\right],\quad\lambda=\frac{2\rho V^2}{kR}.
$$

Subtracting the internal radius obtains

$$
\boxed{\frac hR=H(s)=1-s^{-1/2}+\frac\lambda4(1-s^2),\qquad s=u/V>0}.
$$

This is [choking by wall thickness in an elastic tube](../../../../../choking-by-wall-thickness-in-an-elastic-tube.md). The function tends to $-\infty$ as either $s\downarrow0$ or $s\to\infty$, and $H(1)=0$. Its derivative is

$$
H'(s)=\frac12s^{-3/2}-\frac\lambda2s,
\qquad H'(s)=0\iff s=s_c=\lambda^{-2/5}.
$$

It is positive before $s_c$ and negative afterwards, so the unique maximum is

$$
\boxed{\frac{h_c(\lambda)}R=H(s_c)=1+\frac\lambda4-\frac54\lambda^{1/5},\qquad
u_c=V\lambda^{-2/5}}.
$$

The maximum is nonnegative because the arithmetic-geometric mean inequality gives $4+\lambda\ge5\lambda^{1/5}$; it is zero only at $\lambda=1$. If any prescribed thickness exceeds $h_c$, no positive velocity can satisfy the mass/Bernoulli conditions there, so no flow of this assumed form is possible. Equality is the double-root critical case.

For each $h<h_c$, strict monotonicity on $(0,s_c)$ and $(s_c,\infty)$, together with the two negative-infinite limits, gives exactly two positive roots. The upstream condition is $s\to1$ as $h\to0$. Therefore

$$
\boxed{\begin{array}{c|c|c}
\lambda&\text{selected root}&\text{response to increasing }h\\\hline
0<\lambda<1&s<s_c&u>V\text{ increases}\\
\lambda>1&s>s_c&u<V\text{ decreases}
\end{array}}.
$$

For $\lambda<1$, the upstream value $1$ lies on the rising branch; for $\lambda>1$, it lies on the falling branch. Smooth continuation preserves this choice because the branches meet only at $h_c$, which is excluded by the strict bound. At $\lambda=1$ the upstream state is already critical: $h_c=0$, so the requirement $0\le h<h_c$ cannot hold, and any positive wall thickness is incompatible with the approximation. With $h=0$ the critical root is $u=V$.

<a id="18c/image-velocity-branches-and-critical-wall-thickness-for-steady-flow-through-an-elastic-tube"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3-elastic-tube-choking.png)

**[Figure 1](#18c/image-velocity-branches-and-critical-wall-thickness-for-steady-flow-through-an-elastic-tube). Velocity branches and critical wall thickness for steady flow through an elastic tube**.

The graph shows the unique maximum and the upstream point $(s,H)=(1,0)$ on the three parameter regimes. Only the portion with $H\ge0$ represents nonnegative wall thickness. The vertical maximum line separates the two roots when the prescribed thickness lies strictly below the maximum.

## ↑ Ancestors (10)

1. [18C](../18c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
