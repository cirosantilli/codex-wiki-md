<h1 id="21h/solution">Solution</h1>

↑ **Parent:** [21H](../21h.md)

For an open cover $X=A\cup B$, the [Mayer–Vietoris theorem](../../../../../mayer-vietoris-sequence.md) gives the long exact sequence

$$
\cdots\to H_j(A\cap B)\xrightarrow{(i_*,-j_*)}H_j(A)\oplus H_j(B)\to H_j(X)\to H_{j-1}(A\cap B)\to\cdots.
$$

The same sequence holds for a union of simplicial subcomplexes. All [homology groups](../../../../../homology-group.md) here have [integer](../../../../../integer.md) coefficients.

An explicit [triangulation](../../../../../triangulation.md) of $X_q$ is as follows. Take vertices $b_0,b_1,b_2$ forming a target circle, a circle of $3q$ vertices $a_0,\ldots,a_{3q-1}$, and a cone [vertex](../../../../../vertex-graph-theory.md) $c$. With subscripts on $a$ interpreted modulo $3q$ and on $b$ modulo three, include triangles

$$
[a_j,a_{j+1},b_{j+1}],\qquad[a_j,b_{j+1},b_j],\qquad[c,a_j,a_{j+1}]
$$

for every $j$, together with all their faces. The first two types triangulate the [mapping cylinder](../../../../../mapping-cylinder.md) of the degree-$q$ covering $a_j\mapsto b_j$; the last type fills the inner circle by a disc. A filled disc with an attached annular collar is still a disc, and identifying the outer collar boundary by this covering gives exactly the source quotient. Distinct inner vertices ensure this is a genuine [simplicial complex](../../../../../simplicial-complex.md), not just a one-cell presentation.

Let $A$ be the [mapping cylinder](../../../../../mapping-cylinder.md) and $B$ the coned disc. Then $A$ retracts to the target circle, $B$ is contractible and $A\cap B$ is the inner circle. Its inclusion into $A$ induces multiplication by $q$ on $H_1$. The exact sequence therefore reduces to

$$
0\to H_2(X_q)\to\mathbb Z\xrightarrow{q}\mathbb Z\to H_1(X_q)\to0.
$$

Connectedness and the absence of higher-dimensional simplices give

$$
\boxed{H_0(X_q)=\mathbb Z,\qquad H_1(X_q)=\mathbb Z/q\mathbb Z,\qquad H_j(X_q)=0\quad(j\ge2).}
$$

This is a two-dimensional [Moore space](../../../../../moore-space-algebraic-topology.md) with torsion in degree one.

The [suspension](../../../../../suspension-topology.md) of a connected complex is the union of two cones whose intersection retracts to the original complex. Reduced Mayer-Vietoris gives

$$
\boxed{\widetilde H_j(SK)\cong\widetilde H_{j-1}(K)\quad(j\ge1),\qquad H_0(SK)=\mathbb Z.}
$$

In particular its $H_1$ vanishes. For the wedge of two connected polyhedra, choose neighborhoods retracting onto the two summands with contractible intersection at the wedge point. Then

$$
\boxed{\widetilde H_j(X\vee Y)\cong\widetilde H_j(X)\oplus\widetilde H_j(Y).}
$$

Decompose each prescribed $G_i$ into cyclic summands. Realize each infinite cyclic summand in degree $i$ by $S^i$, and each finite nontrivial summand $\mathbb Z/q$ by $S^{i-1}X_q$, meaning $i-1$ successive [suspensions](../../../../../suspension-topology.md). Take their finite wedge, or a point if there are no summands. The [suspension](../../../../../suspension-topology.md) formula shifts the torsion to degree $i$ and creates no other positive-degree homology, while the wedge formula adds summands. Thus the resulting connected [polyhedron](../../../../../polyhedron.md) satisfies **$\boxed{H_0(X)=\mathbb Z,\ H_i(X)=G_i\ (1\le i\le n),\ H_i(X)=0\ (i>n)}$**. The finite [triangulations](../../../../../triangulation.md) above, their simplicial [suspensions](../../../../../suspension-topology.md) and wedges provide an actual [polyhedron](../../../../../polyhedron.md).

## ↑ Ancestors (10)

1. [21H](../21h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
