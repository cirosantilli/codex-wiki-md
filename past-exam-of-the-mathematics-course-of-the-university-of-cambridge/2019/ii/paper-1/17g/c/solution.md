<h1 id="17g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an eigenvector $v$ with eigenvalue $\theta\in\{\lambda,\mu\}$,

$$
Bv=(A-\lambda I)(A-\mu I)v
=(\theta-\lambda)(\theta-\mu)v=0.
$$

By part (a), every vector orthogonal to $\mathbf e$ is a linear combination of such eigenvectors, so $B$ vanishes on $\mathbf e^\perp$. On the remaining eigenspace,

$$
B\mathbf e=(d-\lambda)(d-\mu)\mathbf e.
$$

The [orthogonal projection](../../../../../../orthogonal-projection.md) onto $\operatorname{span}\{\mathbf e\}$ is $J/n$. It follows that

$$
\boxed{B=\frac{(d-\lambda)(d-\mu)}nJ}.
$$

Put $\kappa=(d-\lambda)(d-\mu)/n$. For $i\ne j$, the identity $B=\kappa J$ reads

$$
(A^2)_{ij}-(\lambda+\mu)A_{ij}=\kappa,
$$

and therefore

$$
(A^2)_{ij}=
\begin{cases}
\kappa+\lambda+\mu,&i\text{ and }j\text{ adjacent},\\
\kappa,&i\text{ and }j\text{ nonadjacent}.
\end{cases}
$$

Because $(A^2)_{ij}$ is the number of common neighbours, these two constants prove that $G$ is strongly regular. This is the converse half of the [three-eigenvalue characterization of a connected strongly regular graph](../../../../../../three-eigenvalue-characterization-of-a-connected-strongly-regular-graph.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17G](../../17g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
