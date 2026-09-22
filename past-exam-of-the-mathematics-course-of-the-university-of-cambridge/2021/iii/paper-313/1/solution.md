<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $N=(0,\ldots,0,1)$ and $S=(0,\ldots,0,-1)$ be the poles of $S^n$. The open sets $U_N=S^n\setminus\{N\}$ and $U_S=S^n\setminus\{S\}$ cover the sphere. [Stereographic projection](../../../../../stereographic-projection.md) gives coordinate charts

$$
\phi_N(r)=\frac{(r_1,\ldots,r_n)}{1-r_{n+1}},
\qquad
\phi_S(r)=\frac{(r_1,\ldots,r_n)}{1+r_{n+1}}
$$

from these sets to $\mathbb R^n$. Their inverses are

$$
\phi_N^{-1}(x)=\left(\frac{2x}{1+|x|^2},
\frac{|x|^2-1}{1+|x|^2}\right),
\qquad
\phi_S^{-1}(y)=\left(\frac{2y}{1+|y|^2},
\frac{1-|y|^2}{1+|y|^2}\right).
$$

On the overlap, the transition map is

$$
\boxed{y=\phi_S\phi_N^{-1}(x)=\frac{x}{|x|^2}},
\qquad x\neq0,
$$

which is a smooth [diffeomorphism](../../../../../diffeomorphism.md) of $\mathbb R^n\setminus\{0\}$. These two compatible charts make $S^n$ a [smooth manifold](../../../../../smooth-manifold.md) of dimension $n$.

Now let $G$ be an $m$-dimensional [Lie group](../../../../../lie-group.md) and choose a basis $e_1,\ldots,e_m$ of its [tangent space](../../../../../tangent-space.md) $T_eG$ at the identity. Define

$$
E_i(g)=(dL_g)_e e_i,
$$

where $L_g$ is [Left translation on a Lie group](../../../../../left-and-right-translation-on-a-lie-group.md). Smoothness of multiplication makes each $E_i$ a smooth [left-invariant vector field](../../../../../left-invariant-vector-field.md), and invertibility of $(dL_g)_e$ makes $E_1(g),\ldots,E_m(g)$ a basis of $T_gG$ at every point. Thus the $E_i$ form a global frame and every Lie group is a [parallelizable manifold](../../../../../parallelizable-manifold.md).

The columns of a matrix in the [special unitary group](../../../../../special-unitary-group.md) $SU(2)$ are orthonormal and its determinant is one. Consequently every element has the unique form

$$
\boxed{U=\begin{pmatrix}
z_1&-\overline z_2\\
z_2&\overline z_1
\end{pmatrix},
\qquad |z_1|^2+|z_2|^2=1}.
$$

The pair $(z_1,z_2)\in\mathbb C^2\cong\mathbb R^4$ therefore identifies $SU(2)$ diffeomorphically with $S^3$. The Lie-group construction then proves that $S^3$ is parallelizable; this is the [SU(2) as the three-sphere](../../../../../su-2-as-the-three-sphere.md) identification.

Another example is $S^1$, which is the Lie group $U(1)$. Explicitly, at $(x,y)\in S^1$ the vector

$$
E(x,y)=-y\frac{\partial}{\partial x}+x\frac{\partial}{\partial y}
$$

is smooth, tangent, and nowhere zero, so it is a global one-vector frame. Thus $S^1$ is another [parallelizable sphere](../../../../../parallelizable-sphere.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 313](../../paper-313-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
