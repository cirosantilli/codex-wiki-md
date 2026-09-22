<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [special orthogonal group](../../../../../special-orthogonal-group.md) in three dimensions is

$$
SO(3)=\{A\in M_3(\mathbb R):A^TA=I,\ \det A=1\}.
$$

Differentiating $A(t)^TA(t)=I$ at the identity shows that its [Lie algebra](../../../../../lie-algebra-split.md) is the space of [skew-symmetric matrices](../../../../../skew-symmetric-matrix.md). A convenient basis is

$$
J_1=\begin{pmatrix}0&0&0\\0&0&-1\\0&1&0\end{pmatrix},
\quad
J_2=\begin{pmatrix}0&0&1\\0&0&0\\-1&0&0\end{pmatrix},
\quad
J_3=\begin{pmatrix}0&-1&0\\1&0&0\\0&0&0\end{pmatrix},
$$

with $[J_a,J_b]=\epsilon_{abc}J_c$.

The infinitesimal action of $\exp(tJ_a)$ on a point $x\in\mathbb R^3$ is $J_ax=e_a\times x$. It therefore generates the vector field

$$
\boxed{V_a=\epsilon_{abc}x_b\frac{\partial}{\partial x_c}}.
$$

Fundamental vector fields for this left action form an antihomomorphism with the stated convention, and direct differentiation gives

$$
\boxed{[V_a,V_b]=-\epsilon_{abc}V_c},
$$

so their span is closed under the [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md).

The brackets $\{x,y\}=z$, $\{y,z\}=x$, and $\{z,x\}=y$ define the [rotational Lie-Poisson structure on R3](../../../../../rotational-lie-poisson-structure-on-r3.md). With the convention that a [Hamiltonian vector field](../../../../../hamiltonian-vector-field.md) acts by $X_H(f)=\{f,H\}$,

$$
X_{x_a}(x_c)=\{x_c,x_a\}=\epsilon_{abc}x_b=V_a(x_c).
$$

Hence the required Hamiltonians are simply

$$
\boxed{H_a=x_a}.
$$

The quadratic function

$$
\boxed{F=x^2+y^2+z^2}
$$

satisfies $\{F,x_a\}=0$ for all $a$, so it is a [Casimir function of a Poisson manifold](../../../../../casimir-function-of-a-poisson-manifold.md). Its nonzero regular level sets $F=R^2$ are spheres. The Poisson tensor has rank two there and is tangent to each level set, so it inverts to a [symplectic form](../../../../../symplectic-form.md); each sphere is a [symplectic leaf](../../../../../symplectic-leaf.md). Rotations preserve both $F$ and the alternating tensor $\epsilon_{abc}$, hence preserve the restricted Poisson tensor and its inverse symplectic form. The $SO(3)$ action therefore restricts to a symplectic action on every sphere $S_R^2\subset\mathbb R^3$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 313](../../paper-313-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
