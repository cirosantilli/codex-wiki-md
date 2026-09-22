<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [Poisson manifold](../../../../../poisson-manifold.md) is a smooth [manifold](../../../../../topological-manifold.md) with an antisymmetric contravariant [tensor field](../../../../../tensor-field.md) $\pi=\tfrac12\pi^{ij}\partial_i\wedge\partial_j$ such that the bracket

$$
\{f,g\}=\pi^{ij}(\partial_i f)(\partial_j g)
$$

satisfies the [Jacobi identity](../../../../../jacobi-identity.md). Bilinearity, antisymmetry and the [Leibniz rule](../../../../../leibniz-rule.md) follow directly from this formula. The [Poisson bivector](../../../../../poisson-bivector.md) is allowed to be degenerate.

Apply the [Jacobi identity](../../../../../jacobi-identity.md) to coordinate functions $x^i,x^j,x^k$. Necessity gives the [coordinate Jacobi condition for a Poisson bivector](../../../../../coordinate-jacobi-condition-for-a-poisson-bivector.md):

$$
\boxed{J^{ijk}:=\pi^{i\ell}\partial_\ell\pi^{jk}+\pi^{j\ell}\partial_\ell\pi^{ki}+\pi^{k\ell}\partial_\ell\pi^{ij}=0.}
$$

For sufficiency, expand $\{f,\{g,h\}\}+\{g,\{h,f\}\}+\{h,\{f,g\}\}$. The terms differentiating $\pi$ are $J^{ijk}f_i g_j h_k$. All terms containing second derivatives cancel. For example, those containing $g_{j\ell}$ have coefficient $(\pi^{i\ell}\pi^{jk}+\pi^{k\ell}\pi^{ij})f_i h_k$, which is antisymmetric under $j\leftrightarrow\ell$ after contraction with $f_i h_k$, whereas $g_{j\ell}$ is symmetric. The same argument handles the second derivatives of $f$ and $h$. Thus the displayed condition is both necessary and sufficient.

A [symplectic manifold](../../../../../symplectic-manifold.md) has a smooth nondegenerate [closed differential form](../../../../../closed-differential-form.md) $\Omega$ of degree two. Write $\Omega=\tfrac12\Omega_{ij}dx^i\wedge dx^j$ and choose the explicit inverse convention $\pi^{ik}\Omega_{kj}=\delta^i_j$. This defines a smooth antisymmetric [bivector](../../../../../bivector.md). Differentiating the inverse matrix gives

$$
\partial_\ell\pi^{ij}=-\pi^{ia}(\partial_\ell\Omega_{ab})\pi^{bj}.
$$

Substitution into the Jacobi coefficient, followed by relabeling summed indices, gives

$$
J^{ijk}=\pi^{ia}\pi^{jb}\pi^{kc}\big(\partial_a\Omega_{bc}+\partial_b\Omega_{ca}+\partial_c\Omega_{ab}\big)=0,
$$

since the parentheses are the components of $d\Omega$. Hence **every symplectic manifold carries a Poisson structure**. The opposite overall convention for the inverse bracket gives the same conclusion. Nondegeneracy and closure together are crucial; an arbitrary invertible antisymmetric tensor need not satisfy the [Jacobi identity](../../../../../jacobi-identity.md).

For a finite-dimensional [Lie algebra](../../../../../lie-algebra-split.md) $\mathfrak g$, its [dual space](../../../../../dual-space.md) $\mathfrak g^*$ carries the [Lie-Poisson bracket](../../../../../lie-poisson-bracket.md)

$$
\{f,g\}(\ell)=\ell([df_\ell,dg_\ell]),
$$

where $df_\ell,dg_\ell$ are identified with elements of $\mathfrak g$. If $[e_i,e_j]=c_{ij}{}^k e_k$ and $x_i(\ell)=\ell(e_i)$, this reads $\{x_i,x_j\}=c_{ij}{}^k x_k$. The Jacobi coefficient is

$$
\big(c_{i\ell}{}^m c_{jk}{}^\ell+c_{j\ell}{}^m c_{ki}{}^\ell+c_{k\ell}{}^m c_{ij}{}^\ell\big)x_m,
$$

which vanishes by the [Lie algebra](../../../../../lie-algebra-split.md) [Jacobi identity](../../../../../jacobi-identity.md).

In particular, the dual of $\mathfrak{so}(3)$ is $\mathbb R^3$ with the [rotational Lie-Poisson structure on R3](../../../../../rotational-lie-poisson-structure-on-r3.md),

$$
\{x,y\}=z,\quad\{y,z\}=x,\quad\{z,x\}=y,\qquad
(\pi^{ij})=\begin{pmatrix}0&z&-y\\-z&0&x\\y&-x&0\end{pmatrix}.
$$

The [Poisson bivector](../../../../../poisson-bivector.md) has rank two away from the origin and rank zero at the origin. The function $x^2+y^2+z^2$ is a [Casimir function](../../../../../casimir-function-of-a-poisson-manifold.md), since its bracket with every function vanishes. The centred spheres are its two-dimensional [symplectic leaves](../../../../../symplectic-leaf.md), and the origin is a point leaf. **This is a Poisson manifold but not a symplectic manifold**: its bivector is not invertible, and an odd-dimensional manifold cannot have a nondegenerate alternating [bilinear form](../../../../../bilinear-form.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
