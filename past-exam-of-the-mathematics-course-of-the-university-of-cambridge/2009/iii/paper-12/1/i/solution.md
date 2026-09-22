<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take a [compactly supported](../../../../../../compact-support.md) smooth variation $\varphi\in C_c^\infty(\Omega)$ and set $u_t=u+t\varphi$. Its support is away from the boundary, so it preserves any prescribed boundary values. Differentiating the [functional](../../../../../../functional.md) at $t=0$ gives the [first variation](../../../../../../first-variation.md)

$$
0=\left.\frac{d}{dt}\mathcal F(u_t)\right|_{t=0}=\int_\Omega\left[F_z(x,u,Du)\varphi+F_{p_i}(x,u,Du)D_i\varphi\right]dx.
$$

By [integration by parts](../../../../../../integration-by-parts.md), there is no boundary term. The [fundamental lemma of the calculus of variations](../../../../../../fundamental-lemma-of-the-calculus-of-variations.md) therefore gives the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md)

$$
\boxed{D_i\bigl(F_{p_i}(x,u,Du)\bigr)=F_z(x,u,Du)\quad\text{in }\Omega.}
$$

Expanding the total derivative, an equivalent classical form is

$$
\boxed{F_{p_ip_j}(x,u,Du)D_{ij}u+F_{p_i z}(x,u,Du)D_i u+F_{p_i x_i}(x,u,Du)-F_z(x,u,Du)=0.}
$$

Repeated indices are summed. In the last term involving $x_i$, the derivative holds $z,p$ fixed; the other terms account for their dependence on $u(x),Du(x)$. [Compactly supported](../../../../../../compact-support.md) variations derive the interior equation without imposing a natural boundary condition.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
