<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $\dot{\mathbf x}=\dot b\,\mathbf u$ and $\varphi=Cb\psi/a$, where the growing [linear growth factor](../../../../../../linear-growth-factor.md) obeys $\ddot b+2H\dot b=Cb/a^3$. The Poisson relation in part (a) immediately becomes

$$
\boxed{\nabla_x^2\psi=\delta/b.}
$$

Along a fluid trajectory,

$$
\ddot{\mathbf x}=\ddot b\,\mathbf u+\dot b^2D_b\mathbf u,\qquad
D_b=\partial_b+\mathbf u\cdot\nabla_x.
$$

Substitute this into the pressureless equation of motion to obtain

$$
\dot b^2D_b\mathbf u+(\ddot b+2H\dot b)\mathbf u
=-\frac{Cb}{a^3}\nabla_x\psi.
$$

The growth equation cancels the second coefficient. By the definition of the logarithmic growth rate, $\dot b=Hbf$, while $C/a^3=(3/2)H^2\Omega(t)$. Therefore

$$
\boxed{D_b\mathbf u=-\frac{3\Omega(t)}{2bf^2}(\mathbf u+\nabla_x\psi).}
$$

This is the printed $d\mathbf u/db$ when interpreted along the particle. Dividing the Eulerian continuity equation by $\dot b$ instead gives

$$
\boxed{\partial_b\delta+\nabla_x\cdot[(1+\delta)\mathbf u]=0.}
$$

The density derivative in this conservative equation must be Eulerian. If both derivatives were read as material derivatives, the density equation would double-count advection; its material form is $D_b\delta+(1+\delta)\nabla_x\cdot\mathbf u=0$. These distinctions make the [growth-time form of cosmological dust equations](../../../../../../growth-time-form-of-cosmological-dust-equations.md) valid beyond the first-order terms, up to the single-stream pressureless-fluid limit. The reparameterization assumes $\dot b\ne0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
