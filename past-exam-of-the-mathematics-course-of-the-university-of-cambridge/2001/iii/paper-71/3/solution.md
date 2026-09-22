<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [symplectic manifold](../../../../../symplectic-manifold.md) is a smooth even-dimensional [manifold](../../../../../topological-manifold.md) $M$ with a [differential two-form](../../../../../2-form.md) $\omega$ that is closed, $d\omega=0$, and nondegenerate at every point. Nondegeneracy identifies [vector fields](../../../../../vector-field.md) with [differential one-forms](../../../../../one-form.md) by the [interior product](../../../../../interior-product.md) $X\mapsto\iota_X\omega$. In this solution use the explicit [Hamiltonian vector field](../../../../../hamiltonian-vector-field.md) convention

$$
\iota_{X_f}\omega=df,\qquad \{f,g\}=\omega(X_f,X_g).
$$

This contraction sign differs from the negative-sign convention sometimes used for [Hamiltonian vector fields](../../../../../hamiltonian-vector-field.md); all subsequent signs are fixed by the displayed choice. In [Darboux coordinates](../../../../../darboux-chart.md) with $\omega=\sum_a dx_a\wedge dy_a$ it gives

$$
X_f=\sum_a\left(f_{y_a}\partial_{x_a}-f_{x_a}\partial_{y_a}\right),\qquad \{f,g\}=\sum_a\left(f_{x_a}g_{y_a}-f_{y_a}g_{x_a}\right),\qquad X_f(g)=-\{f,g\}.
$$

The [Poisson bracket](../../../../../poisson-bracket.md) is bilinear and antisymmetric, and the ordinary product rule gives $\{f,gh\}=\{f,g\}h+g\{f,h\}$. Thus it remains to check the [Jacobi identity for the Poisson bracket](../../../../../jacobi-identity-for-the-poisson-bracket.md).

The [Cartan formula for the Lie derivative](../../../../../cartan-s-magic-formula.md) and closedness of the [symplectic form](../../../../../symplectic-form.md) give $\mathcal L_{X_f}\omega=d(\iota_{X_f}\omega)+\iota_{X_f}d\omega=d^2f=0$. Hence

$$
\begin{aligned}
\iota_{[X_f,X_g]}\omega&=\mathcal L_{X_f}(\iota_{X_g}\omega)-\iota_{X_g}(\mathcal L_{X_f}\omega)\\
&=\mathcal L_{X_f}(dg)=d(X_f g)=-d\{f,g\},
\end{aligned}
$$

and nondegeneracy gives

$$
\boxed{[X_f,X_g]=-X_{\{f,g\}}.}
$$

Applying both sides to an arbitrary smooth function $h$ gives $\{f,\{g,h\}\}-\{g,\{f,h\}\}=\{\{f,g\},h\}$, which is exactly the [Jacobi identity for the Poisson bracket](../../../../../jacobi-identity-for-the-poisson-bracket.md). Consequently the smooth functions, with their pointwise product and this [Poisson bracket](../../../../../poisson-bracket.md), form a [Poisson algebra](../../../../../poisson-algebra.md). Constants have zero [Hamiltonian vector field](../../../../../hamiltonian-vector-field.md). If $f,g$ are components of [moment maps](../../../../../moment-map.md), the same displayed relation relates the brackets of their [Hamiltonian vector fields](../../../../../hamiltonian-vector-field.md) to the [Poisson bracket](../../../../../poisson-bracket.md) of those components. In the opposite contraction convention the corresponding relation is the [Hamiltonian Lie algebra homomorphism](../../../../../hamiltonian-lie-algebra-homomorphism.md) with the compatible bracket sign.

For the [point vortices](../../../../../line-vortex.md), remove the collision diagonals from $(\mathbb R^2)^N$, since the logarithmic [Hamiltonian function](../../../../../hamiltonian-function.md) is singular there. Set $s_{ab}=(x_a-x_b)^2+(y_a-y_b)^2>0$ for $a\ne b$. Differentiating each pair contribution gives

$$
H_{x_a}=-2\sum_{b\ne a}\frac{x_a-x_b}{s_{ab}},\qquad H_{y_a}=-2\sum_{b\ne a}\frac{y_a-y_b}{s_{ab}}.
$$

The [Hamiltonian vector field](../../../../../hamiltonian-vector-field.md) therefore gives the equations of motion

$$
\boxed{\dot x_a=-2\sum_{b\ne a}\frac{y_a-y_b}{s_{ab}},\qquad\dot y_a=2\sum_{b\ne a}\frac{x_a-x_b}{s_{ab}}.}
$$

Each contribution is perpendicular to the displacement from vortex $b$ to vortex $a$ and has magnitude $2/|\mathbf r_a-\mathbf r_b|$. This is the velocity induced by a [point vortex](../../../../../line-vortex.md) of positive [circulation](../../../../../circulation-physics.md), with the normalization $\Gamma/(2\pi)=2$. Each vortex is advected by the velocity of the others, without a self-induced singular velocity. Pairwise contributions cancel in the total velocity, so $\sum_a x_a$ and $\sum_a y_a$ are conserved. For two vortices the separation is constant and they rotate counterclockwise about their midpoint, as expected for identical positive [point vortices](../../../../../line-vortex.md).

For $L=\tfrac12\sum_a(x_a^2+y_a^2)$, compute its [Poisson bracket](../../../../../poisson-bracket.md) with $H$ directly:

$$
\{L,H\}=\sum_a(x_aH_{y_a}-y_aH_{x_a})=-2\sum_a\sum_{b\ne a}\frac{y_ax_b-x_ay_b}{s_{ab}}=0.
$$

The last sum vanishes by pairing $(a,b)$ with $(b,a)$, since their numerators are opposite and denominators equal. Thus **$L$ Poisson commutes with $H$ and is conserved**. Equivalently, the [Hamiltonian function](../../../../../hamiltonian-function.md) depends only on pairwise distances and is invariant under simultaneous rotations.

The standard positive generator of the simultaneous [circle group](../../../../../circle-group.md) $SO(2)$ action is

$$
Y=\sum_a\left(-y_a\partial_{x_a}+x_a\partial_{y_a}\right).
$$

Its [interior product](../../../../../interior-product.md) with the [symplectic form](../../../../../symplectic-form.md) is

$$
\iota_Y\omega=-\sum_a(y_a\,dy_a+x_a\,dx_a)=-dL.
$$

Use the [moment map](../../../../../moment-map.md) convention $d\langle\mu,\xi\rangle=-\iota_{Y_\xi}\omega$ for the usual positive rotation generator. Identifying $\mathfrak{so}(2)^*$ with $\mathbb R$, this proves **$L$ is the moment map for the standard rotation action**. It is invariant under the action, hence equivariant because [circle group](../../../../../circle-group.md) $SO(2)$ is abelian. Additive constants are possible; the natural normalization is $L=0$ at the origin of the ambient space. On the collision-free space this polynomial is its restriction. With the solution's positive contraction convention, the rotation generator is $Y=-X_L$. Confusing these two signs would reverse the final augmented Hamiltonian.

Let $\mathcal R_\varphi$ denote simultaneous counterclockwise rotation through $\varphi$, and introduce the co-rotating coordinates by $\mathbf r(t)=\mathcal R_{\Omega t}\mathbf r'(t)$. Both the [symplectic form](../../../../../symplectic-form.md) and $H$ are rotation-invariant, so pulling back the inertial [Hamiltonian vector field](../../../../../hamiltonian-vector-field.md) leaves $X_H$ unchanged. Differentiating the rotation gives the co-rotating equation

$$
\dot{\mathbf r}'=X_H(\mathbf r')-\Omega Y(\mathbf r')=X_H(\mathbf r')+\Omega X_L(\mathbf r')=X_{H+\Omega L}(\mathbf r').
$$

The co-rotating positions are constant precisely when this [Hamiltonian vector field](../../../../../hamiltonian-vector-field.md) vanishes. By nondegeneracy of the [symplectic form](../../../../../symplectic-form.md), that is equivalent to

$$
\boxed{d(H+\Omega L)(\mathbf r')=0.}
$$

Conversely a collision-free [critical point](../../../../../critical-point.md) of this augmented [Hamiltonian function](../../../../../hamiltonian-function.md) produces a rigidly rotating solution. This is a [rotating point-vortex relative equilibrium](../../../../../rotating-point-vortex-relative-equilibrium.md).

As a sign and scaling check, scaling every position by $s>0$ changes $H$ by $-N(N-1)\log s$. Therefore $\sum_a\mathbf r_a\cdot\nabla_aH=-N(N-1)$. At a [rotating point-vortex relative equilibrium](../../../../../rotating-point-vortex-relative-equilibrium.md), $\nabla_aH+\Omega\mathbf r_a=0$, so $2\Omega L=N(N-1)$. For $N\geq2$ the [angular velocity](../../../../../angular-velocity.md) is positive in this circulation convention. An equilateral three-vortex configuration of circumradius $\rho$ has $L=3\rho^2/2$ and $\Omega=2/\rho^2$, agreeing directly with the equations of motion.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
