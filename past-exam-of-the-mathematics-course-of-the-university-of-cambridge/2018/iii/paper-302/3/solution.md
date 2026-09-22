<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the wiki's [Cartan matrix](../../../../../cartan-matrix.md) convention

$$
A_{ij}=\langle\alpha_i,\alpha_j^\vee\rangle=\frac{2(\alpha_i,\alpha_j)}{(\alpha_j,\alpha_j)}.
$$

Label the long [simple root](../../../../../simple-root.md) first when the lengths differ. The matrix of an irreducible rank-two [root system](../../../../../root-system.md) has the form $A=\begin{pmatrix}2&-a\\-b&2\end{pmatrix}$, where $a,b$ are positive integers. Integrality and the signs follow from the [Cartan integers](../../../../../cartan-integer.md) for distinct simple roots, and irreducibility rules out a zero off-diagonal pair. Its positive-definite symmetrization gives $ab<4$, equivalently $ab=4\cos^2\theta<4$. Moreover $a/b=\|\alpha_1\|^2/\|\alpha_2\|^2\geq1$. Thus $(a,b)=(1,1),(2,1),(3,1)$, giving the entire [classification of rank-two root systems](../../../../../classification-of-rank-two-root-systems.md) relevant to a simple algebra:

$$
\boxed{\begin{array}{c|c|c|c}
\text{type}&A&\|\alpha_1\|/\|\alpha_2\|&\theta\\\hline
A_2&\begin{pmatrix}2&-1\\-1&2\end{pmatrix}&1&2\pi/3\\
B_2=C_2&\begin{pmatrix}2&-2\\-1&2\end{pmatrix}&\sqrt2&3\pi/4\\
G_2&\begin{pmatrix}2&-3\\-1&2\end{pmatrix}&\sqrt3&5\pi/6
\end{array}}
$$

These correspond to $\mathfrak{sl}_3(\mathbb C)$, $\mathfrak{so}_5(\mathbb C)\cong\mathfrak{sp}_4(\mathbb C)$, and the exceptional algebra $\mathfrak g_2$. Here $B_2=C_2$ denotes the [Isomorphism between so5 and sp4](../../../../../isomorphism-between-so5-and-sp4.md), not an additional case. The disconnected $A_1\times A_1$ system corresponds to a semisimple but nonsimple algebra and is excluded.

The [Dynkin diagrams](../../../../../dynkin-diagram.md), with nodes in the same order as the matrices, are

$$
\begin{array}{ccl}
A_2&:&\overset{\alpha_1}{\circ}\! -\!\overset{\alpha_2}{\circ},\\[0.5em]
B_2&:&\overset{\alpha_1}{\circ}\!\Rightarrow\!\overset{\alpha_2}{\circ},\\[0.5em]
G_2&:&\overset{\alpha_1}{\circ}\!\equiv\!>\!\overset{\alpha_2}{\circ}.
\end{array}
$$

The second and third diagrams have two and three bonds respectively, with the arrowhead pointing to the [short root](../../../../../short-root.md) $\alpha_2$. In the last diagram $\equiv$ draws the three bonds and $>$ their arrowhead.

To enumerate roots, use the standard [root string](../../../../../root-string.md) theorem: for $\beta\ne\pm\alpha$, the roots $\beta+n\alpha$ are consecutive from $\beta-p\alpha$ through $\beta+q\alpha$, with $p-q=\langle\beta,\alpha^\vee\rangle$. Also use the standard results that the [root system](../../../../../root-system.md) is reduced, every root is conjugate under the [Weyl group](../../../../../weyl-group.md) to a simple root, and each [root space](../../../../../root-space.md) has dimension one.

Write $m=a\in\{1,2,3\}$. Since a difference of simple roots is not a root, the $\alpha_2$-string starting at $\alpha_1$ has $p=0$ and $q=m$. It produces $\alpha_1,\alpha_1+\alpha_2,\ldots,\alpha_1+m\alpha_2$. The $\alpha_1$-string starting at $\alpha_2$ has $q=1$. In type $G_2$, the further string through $\beta=\alpha_1+3\alpha_2$ has

$$
\langle\beta,\alpha_1^\vee\rangle=2-3=-1,
$$

and $\beta-\alpha_1=3\alpha_2$ is not a root, so it also produces $2\alpha_1+3\alpha_2$. The resulting positive roots are

$$
\boxed{\begin{aligned}
\Phi^+(A_2)&=\{\alpha_1,\alpha_2,\alpha_1+\alpha_2\},\\
\Phi^+(B_2)&=\{\alpha_1,\alpha_2,\alpha_1+\alpha_2,\alpha_1+2\alpha_2\},\\
\Phi^+(G_2)&=\{\alpha_1,\alpha_2,\alpha_1+\alpha_2,\alpha_1+2\alpha_2,\alpha_1+3\alpha_2,2\alpha_1+3\alpha_2\}.
\end{aligned}}
$$

All roots are these and their negatives. To check completeness, the simple [root reflections](../../../../../root-reflection.md) act on coordinates by

$$
s_1(r\alpha_1+s\alpha_2)=(-r+s)\alpha_1+s\alpha_2,\qquad
s_2(r\alpha_1+s\alpha_2)=r\alpha_1+(mr-s)\alpha_2.
$$

Each listed set together with its negatives is stable under both reflections. It contains the simple roots and consists of roots already forced by strings. Since every root lies in a Weyl orbit of a simple root, no other roots can occur. This proves the lists for the [A2 root system](../../../../../a2-root-system.md), [B2 root system](../../../../../b2-root-system.md), and [G2 root system](../../../../../g2-root-system.md). The [root-space decomposition](../../../../../root-space-decomposition.md) then gives

$$
\boxed{\dim\mathfrak{sl}_3=2+6=8,\qquad\dim\mathfrak{so}_5=2+8=10,\qquad\dim\mathfrak g_2=2+12=14.}
$$

For the restriction to a [sl2 subalgebra associated with a root](../../../../../sl2-subalgebra-associated-with-a-root.md), normalize its Cartan element to be $h_\alpha=\alpha^\vee$. On a root vector of root $\beta$, its eigenvalue is $\langle\beta,\alpha^\vee\rangle$. The [classification of finite-dimensional sl2 representations](../../../../../classification-of-finite-dimensional-sl2-representations.md) says that $R(\Lambda)$ has weights $\Lambda,\Lambda-2,\ldots,-\Lambda$ and dimension $\Lambda+1$. A root string of $\Lambda+1$ nonparallel roots therefore supplies one such irreducible module: the raising and lowering brackets connect its consecutive root spaces.

For clarity, the positive-side strings for each simple-root direction are listed below. Brackets denote the whole consecutive string; a single listed root is a string of length one. In every row also include each negative string in reverse order, and separately the triple formed by the root $\alpha_i$, its negative, and $h_{\alpha_i}$.

$$
\begin{array}{c|c|l}
\text{type}&\text{direction}&\text{nonparallel positive-side strings}\\\hline
A_2&\alpha_1&[\alpha_2,\alpha_1+\alpha_2]\\
A_2&\alpha_2&[\alpha_1,\alpha_1+\alpha_2]\\
B_2&\alpha_1&[\alpha_2,\alpha_1+\alpha_2],\quad[\alpha_1+2\alpha_2]\\
B_2&\alpha_2&[\alpha_1,\alpha_1+\alpha_2,\alpha_1+2\alpha_2]\\
G_2&\alpha_1&[\alpha_2,\alpha_1+\alpha_2],\quad[\alpha_1+3\alpha_2,2\alpha_1+3\alpha_2],\quad[\alpha_1+2\alpha_2]\\
G_2&\alpha_2&[\alpha_1,\alpha_1+\alpha_2,\alpha_1+2\alpha_2,\alpha_1+3\alpha_2],\quad[2\alpha_1+3\alpha_2]
\end{array}
$$

The root's own triple is always $R(2)$. The one-dimensional subspace of $\mathfrak h$ annihilated by $\alpha_i$ commutes with this subalgebra and gives $R(0)$. Each singleton root in the table, and its negative, contributes another $R(0)$. Reading the other string lengths now gives the [adjoint branching to root sl2 subalgebras in rank two](../../../../../adjoint-branching-to-root-sl2-subalgebras-in-rank-two.md):

$$
\boxed{\begin{array}{c|c|l}
\text{type}&\text{simple root}&\mathfrak g\downarrow_{\mathfrak{sl}_2(\alpha_i)}\\\hline
A_2&\alpha_1\text{ or }\alpha_2&R(2)\oplus2R(1)\oplus R(0)\\
B_2&\alpha_1\text{ (long)}&R(2)\oplus2R(1)\oplus3R(0)\\
B_2&\alpha_2\text{ (short)}&3R(2)\oplus R(0)\\
G_2&\alpha_1\text{ (long)}&R(2)\oplus4R(1)\oplus3R(0)\\
G_2&\alpha_2\text{ (short)}&R(2)\oplus2R(3)\oplus3R(0)
\end{array}}
$$

Their dimensions are respectively $8,10,10,14,14$. The last row agrees with [G2 adjoint branching to a short-root sl2 subalgebra](../../../../../g2-adjoint-branching-to-a-short-root-sl2-subalgebra.md). All labels in the table are highest weights, rather than dimensions.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 302](../../paper-302-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
