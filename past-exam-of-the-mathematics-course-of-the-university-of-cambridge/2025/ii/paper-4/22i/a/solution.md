<h1 id="22i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Riesz representation theorem](../../../../../../riesz-representation-theorem.md) says that for every bounded linear functional $f$ on a Hilbert space $H$, there is a unique $z\in H$ such that

$$
f(x)=\langle x,z\rangle\qquad(x\in H),
$$

and $\lVert f\rVert=\lVert z\rVert$.

For $T\in L(H)$ and fixed $y\in H$, the map

$$
f_y(x)=\langle Tx,y\rangle
$$

is a bounded linear functional, with

$$
|f_y(x)|\leq\lVert T\rVert\lVert x\rVert\lVert y\rVert.
$$

Riesz therefore gives a unique vector, denoted $T^*y$, such that

$$
\langle Tx,y\rangle=\langle x,T^*y\rangle
$$

for every $x$. Uniqueness in the representation theorem shows that $y\mapsto T^*y$ is linear. Moreover,

$$
\lVert T^*y\rVert=\lVert f_y\rVert
\leq\lVert T\rVert\lVert y\rVert,
$$

so the [adjoint operator](../../../../../../adjoint-operator.md) belongs to $L(H)$ and $\lVert T^*\rVert\leq\lVert T\rVert$.

If $(e_j)$ is an orthonormal basis and $A=(a_{ij})$ is the matrix of $T$, then the matrix of $T^*$ is

$$
A^*=\overline A^{,T};
$$

its entries are $\overline{a_{ji}}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [22I](../../22i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
