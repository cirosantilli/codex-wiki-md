<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At leading order the particle is a sphere. A pure applied couple produces no translation, while torque balance with the [rotating sphere in Stokes flow](../../../../../../rotating-sphere-in-stokes-flow.md) gives

$$
\boxed{\mathbf U_0=0},
\qquad
\boxed{\boldsymbol\Omega_0=\frac{\mathbf G}{8\pi\mu a^3}}.
$$

With $mathbf n$ directed from the particle into the fluid, the exact conditions on the true surface $S$ are

$$
\mathbf u=\mathbf U+\boldsymbol\Omega\times\mathbf x,
\qquad
\int_S\boldsymbol\sigma\mathbf n\,dS=0,
\qquad
\int_S\mathbf x\times(\boldsymbol\sigma\mathbf n)\,dS=-\mathbf G.
$$

Evaluate no slip at $mathbf x_s=(a+\varepsilon f)\mathbf n$ and expand about $mathbf x=a\mathbf n$. The order-$\varepsilon$ terms give

$$
\boxed{\mathbf u_1=\mathbf U_1+\boldsymbol\Omega_1\times\mathbf x
+\frac fa\boldsymbol\Omega_0\times\mathbf x
-f\frac{\partial\mathbf u_0}{\partial r}}
\qquad(r=a).
$$

The divergence of the Newtonian stress vanishes in the surrounding fluid, and its symmetry makes the divergence of angular-momentum flux vanish as well. The total force and torque may therefore be evaluated on any homologous enclosing surface, in particular the fixed reference sphere. Since the applied force is zero and the applied couple is fixed independently of $\varepsilon$,

$$
\boxed{\int_{r=a}\boldsymbol\sigma_1\mathbf n\,dS=0},
\qquad
\boxed{\int_{r=a}\mathbf x\times(\boldsymbol\sigma_1\mathbf n)\,dS=0}.
$$

Using a fixed enclosing sphere is also why no separate terms involving the shape $f$ and leading stress $\boldsymbol\sigma_0$ appear.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
