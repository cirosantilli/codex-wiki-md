<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A map $p:E\to B$ is a [Serre fibration](../../../../../serre-fibration.md) if every [homotopy](../../../../../homotopy.md) $H:D^k\times I\to B$, $k\ge0$, with a lift of its initial slice has a lift on the whole cylinder extending that initial lift. By attaching cells, this gives the relative [homotopy lifting property](../../../../../homotopy-lifting-property.md) for [CW pairs](../../../../../cw-pair.md): a specified lift on the initial slice and on the subcomplex cylinder can be extended.

Give $PY$ the [compact-open topology](../../../../../compact-open-topology.md). Suppose the initial lifting is a family of paths $\gamma_x$ starting at $y_0$, with $\gamma_x(1)=H(x,0)$. Define

$$
\widetilde H(x,s)(t)=\begin{cases}\gamma_x((1+s)t)&0\le t\le(1+s)^{-1},\\H(x,(1+s)t-1)&(1+s)^{-1}\le t\le1.\end{cases}
$$

The two expressions coincide on their common boundary, the initial path at $s=0$ is exactly $\gamma_x$, and the endpoint is $H(x,s)$. The adjoint map on $D^k\times I\times I$ is continuous by pasting; [compactness](../../../../../compact-space.md) of the path parameter gives continuity into the [path space](../../../../../path-space.md). Thus **endpoint evaluation $PY\to Y$ is a [Serre fibration](../../../../../serre-fibration.md)**. The variable subdivision avoids changing the initial lift by an unwanted reparametrization.

For a based pair $(E,F,e_0)$, the [long exact sequence of relative homotopy groups](../../../../../long-exact-sequence-of-relative-homotopy-groups.md) is

$$
\cdots\to\pi_n(F)\xrightarrow{i_*}\pi_n(E)\xrightarrow{j_*}\pi_n(E,F)\xrightarrow{\partial}\pi_{n-1}(F)\xrightarrow{i_*}\pi_{n-1}(E)\to\cdots,
$$

ending in $\pi_1(E)\to\pi_1(E,F)\to\pi_0(F)\to\pi_0(E)$. The low-dimensional end is an exact sequence of [pointed sets](../../../../../pointed-set.md) with its usual actions, rather than an entirely abelian sequence.

The boundary sends a relative disk map to its restriction on the boundary [sphere](../../../../../sphere.md). An absolute class has constant boundary, so $\partial j_*=0$. Conversely, if a relative map has [null-homotopic](../../../../../null-homotopic-map.md) boundary in $F$, choose a based null-homotopy there. Attach this null-homotopy as a collar to the disk, leaving the original map on a smaller inner disk. The resulting boundary is constant at $e_0$, so it defines an absolute class in $\pi_n(E)$; inserting the collar is a relative [homotopy](../../../../../homotopy.md), so its image is the original relative class. This proves **$\operatorname{im}j_*=\ker\partial$**. At $n=1$, append a path in $F$ from the terminal point to $e_0$, giving the corresponding based loop and pointed-set exactness.

Now suppose $F=p^{-1}(b_0)$. Use a cube model in which the bottom and side faces are based and the top face maps into $F$. A based $n$-cube in $B$ lifts from its constant bottom face, with sides held at $e_0$ by relative lifting. Its top face lies in $F$, proving surjectivity of the [relative homotopy of a Serre fibration](../../../../../relative-homotopy-of-a-serre-fibration.md) comparison $p_*:\pi_n(E,F)\to\pi_n(B,b_0)$.

For injectivity, lift a based [homotopy](../../../../../homotopy.md) of two projected cubes from the first relative lift; this ends at some lift of the second base cube. Any two lifts of that same base cube are relatively homotopic: insert an extra parameter between them, prescribe the two liftings on its two ends and the constant lift on the bottom, and apply relative lifting in the remaining cube direction. The top face stays in $F$ because its projection is $b_0$. Combining these [homotopies](../../../../../homotopy.md) proves injectivity. Therefore

$$
\boxed{p_*:\pi_n(E,F)\xrightarrow{\cong}\pi_n(B,b_0)\quad(n\ge2).}
$$

At $n=1$ the same construction gives a bijection of [pointed sets](../../../../../pointed-set.md), and one can transport the base fundamental-group law across it. An arbitrary pair's relative $\pi_1$ has no general [group](../../../../../group-split.md) law. The printed target index $a$ is a typographical error: the map preserves degree $n$.

The last-column map $U(n)\to S^{2n-1}$ is surjective because a unit vector can be completed to a unitary basis. Its stabilizer is the block subgroup $\operatorname{diag}(U(n-1),1)$, so it induces a continuous bijection $U(n)/U(n-1)\to S^{2n-1}$. [Unitary matrices](../../../../../unitary-matrix.md) form a [compact](../../../../../compact-space.md) set in their matrix-space topology; the quotient is [compact](../../../../../compact-space.md) and the [sphere](../../../../../sphere.md) [Hausdorff](../../../../../hausdorff-space.md). Hence

$$
\boxed{U(n)/U(n-1)\cong S^{2n-1}.}
$$

This quotient is a fiber bundle. Near the last standard unit vector, project the other standard vectors by $I-vv^*$ onto $v^\perp$ and apply [Gram-Schmidt orthogonalization](../../../../../gram-schmidt-process.md); their independence persists in a small neighborhood. The resulting orthonormal columns together with $v$ give a continuous local section. Translating these sections covers the [sphere](../../../../../sphere.md) and trivializes the projection, so it is a [Serre fibration](../../../../../serre-fibration.md).

Apply this to $U(n)\to U(n+1)\to S^{2n+1}$. Its [homotopy](../../../../../homotopy.md) sequence contains

$$
\pi_{i+1}(S^{2n+1})\to\pi_i(U(n))\to\pi_i(U(n+1))\to\pi_i(S^{2n+1}).
$$

For $i\le2n-1$, both outer [groups](../../../../../group-split.md) vanish by [cellular approximation theorem](../../../../../cellular-approximation-theorem.md). Thus **$\pi_i(U(n))\cong\pi_i(U(n+1))$ in the stated range**. The component assertion also holds: diagonalizing a [unitary matrix](../../../../../unitary-matrix.md) and varying its eigenvalue phases continuously connects it to the identity. This establishes the [unitary sphere quotient and stability range](../../../../../unitary-sphere-quotient-and-stability-range.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
