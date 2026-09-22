<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A vertex $i$ of a [quiver](../../../../../quiver.md) is a [sink](../../../../../sink-of-a-quiver.md) when no arrow starts at $i$. A [representation of a quiver](../../../../../representation-of-a-quiver.md) assigns a vector space $V_j$ to every vertex and a linear map $V_a:V_j\to V_\ell$ to every arrow $a:j\to\ell$. A morphism $f:V\to W$ is a family of linear maps $f_j:V_j\to W_j$ such that $f_\ell V_a=W_af_j$ for every arrow. The quiver has [finite representation type](../../../../../finite-representation-type-of-a-quiver.md) when it has only finitely many isomorphism classes of indecomposable finite-dimensional representations.

At a sink $i$, the [Bernstein–Gelfand–Ponomarev reflection functor](../../../../../bernstein-gelfand-ponomarev-reflection-functor.md) replaces

$$
V_i\quad\text{by}\quad
\ker\left(\bigoplus_{a:j\to i}V_j\longrightarrow V_i\right)
$$

and reverses the arrows ending at $i$; the new arrow maps are the kernel inclusion followed by the coordinate projections. Every representation is a direct sum of copies of the simple representation $S_i$ and a representation for which the displayed incoming map is surjective. On the latter representations, reflection at the resulting source, using the corresponding cokernel, is inverse up to natural isomorphism. Thus reflection gives a bijection between indecomposable representations other than $S_i$ on the two sides. Adding the one omitted simple representation on each side proves that reversing all arrows into a sink preserves finite representation type.

For the four-arrow star $Q_1$, take $V_1=\cdots=V_4=k$, $V_5=k^2$, and let the four arrows have images

$$
k(1,0),\quad k(0,1),\quad k(1,1),\quad k(1,\lambda),
\qquad \lambda\in k\setminus\{0,1\}.
$$

An endomorphism must preserve the first two lines, so its map on $V_5$ is diagonal. Preserving the third forces its diagonal entries to agree, and then all vertex maps are multiplication by that same scalar. The endomorphism ring is therefore $k$, so this representation is a [brick module](../../../../../brick-module.md) and hence indecomposable. Any isomorphism between parameters preserves the first three labelled lines; the induced [projective linear transformation](../../../../../projective-linear-transformation.md) is therefore the identity, and the fourth line gives $\lambda=\mu$. Since $k$ is infinite, this is an infinite family of pairwise nonisomorphic indecomposables. Hence $Q_1$ is not of finite representation type. Repeatedly applying the reflection result to sinks or, dually, to sources shows that every orientation obtained by reversing some of its arrows also has infinite representation type.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 102](../../paper-102-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
