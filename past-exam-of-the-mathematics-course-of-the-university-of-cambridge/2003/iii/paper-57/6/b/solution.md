<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every matrix in $SU(2)$ has the unique form

$$
U=\begin{pmatrix}\alpha&\beta\\-\overline\beta&\overline\alpha\end{pmatrix},\qquad |\alpha|^2+|\beta|^2=1.
$$

The four real coordinates of $(\alpha,\beta)$ give a smooth bijection with smooth inverse onto the unit [three-sphere](../../../../../../three-sphere.md). Matrix multiplication identifies this model with the [unit quaternions](../../../../../../unit-quaternion.md). Its round metric is invariant under left and right multiplication by unit quaternions. The action

$$
(a,b):q\longmapsto aqb^{-1}
$$

has kernel $\{(1,1),(-1,-1)\}$: a kernel pair must have $a=b$ from $q=1$ and must commute with all quaternions. Its derivative is injective, and both dimensions are six, giving

$$
\boxed{\operatorname{Isom}_0(S^3)=SO(4)\cong(SU(2)\times SU(2))/\{\pm(I,I)\}.}
$$

The full [isometry group](../../../../../../isometry-group.md) is $O(4)$. Quaternion conjugation reverses orientation and supplies the additional component. Thus an arbitrary isometry has either the displayed left-right form or that form composed with conjugation.

For the [Anti-de Sitter spacetime](../../../../../../anti-de-sitter-spacetime.md) model, write

$$
M=\begin{pmatrix}x_0+x_1&x_2+x_3\\x_2-x_3&x_0-x_1\end{pmatrix},\qquad
-\det M=-x_0^2-x_3^2+x_1^2+x_2^2.
$$

The hyperboloid with this quadratic form equal to $-1$ is exactly $SL(2,\mathbb R)$. Its induced Lorentzian metric is preserved by $M\mapsto AMB^{-1}$ for $A,B\in SL(2,\mathbb R)$. At the identity the metric is $g(U,V)=\tfrac12\operatorname{tr}(UV)$ on traceless matrices, so it is the [Killing metric](../../../../../../killing-form-einstein-metric.md) divided by eight. This proves the geometric identification, including the metric rather than only the underlying manifold.

A trivial left-right action again forces $A=B$ to be a scalar commuting with all determinant-one matrices, hence $A=B=\pm I$. The differential is injective and both dimensions are six, so

$$
\boxed{\operatorname{Isom}_0(\mathrm{AdS}_3)=SO_0(2,2)
\cong(SL(2,\mathbb R)\times SL(2,\mathbb R))/\{\pm(I,I)\}.}
$$

This is the existing [left-right double cover of SO0(2,2)](../../../../../../left-right-double-cover-of-so0-2-2.md). The full hyperboloid [isometry group](../../../../../../isometry-group.md) is $O(2,2)$. Its other components can be obtained by also using $M\mapsto M^T$ and $M\mapsto CMC^{-1}$, $C=\operatorname{diag}(1,-1)$. Transposition reverses one timelike coordinate; conjugation by $C$ reverses one timelike and one spacelike coordinate, so these generate the four component classes. All isometries of these constant-curvature quadrics come from ambient orthogonal transformations: a value and an orthonormal derivative at one point determine an isometry, and the ambient group realizes every such choice.

Here $\mathrm{AdS}_3$ means the hyperboloid with periodic time. The physically common causally unwrapped spacetime is its [universal cover](../../../../../../universal-cover.md), modeled by the [universal covering Lie group](../../../../../../universal-covering-lie-group.md) of $SL(2,\mathbb R)$, and is not itself $SL(2,\mathbb R)$. Its isometries lift the above local symmetries, with the global covering and central identifications changed accordingly.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
