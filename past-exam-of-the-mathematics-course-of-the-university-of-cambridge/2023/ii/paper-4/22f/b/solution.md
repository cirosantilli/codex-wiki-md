<h1 id="22f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $z_n=x_n-x$, so $z_n\rightharpoonup0$. We show that the norm closure of the [convex hull](../../../../../../convex-hull.md) of every tail

$$
A_k=\{z_n:n\geq k\}
$$

contains zero. If it did not, the [Hahn-Banach separation theorem](../../../../../../hahn-banach-separation-theorem.md) would give a bounded linear functional $\phi$, a real number $c>0$, and, after multiplying $\phi$ by a complex scalar if necessary,

$$
\operatorname{Re}\phi(z)\geq c
$$

for every $z$ in that closed convex hull. In particular $\operatorname{Re}\phi(z_n)\geq c$ for all $n\geq k$. By the [Riesz representation theorem](../../../../../../riesz-representation-theorem.md), $\phi(z)=\langle z,y\rangle$ for some $y\in H$, contradicting $z_n\rightharpoonup0$.

Consequently, for every $k$ there is a finite [convex combination](../../../../../../convex-combination.md)

$$
w_k=\sum_{n=k}^{N_k}\lambda_{k,n}z_n,
\qquad
\lambda_{k,n}\geq0,
\qquad
\sum_{n=k}^{N_k}\lambda_{k,n}=1,
$$

with $\lVert w_k\rVert_H<1/k$. Define

$$
\widetilde x_k=x+w_k
=\sum_{n=k}^{N_k}\lambda_{k,n}x_n.
$$

Then every $\widetilde x_k$ is a convex combination of terms of the original sequence and

$$
\lVert\widetilde x_k-x\rVert_H=\lVert w_k\rVert_H<\frac1k\longrightarrow0.
$$

This is [Mazur lemma](../../../../../../mazur-s-lemma.md) in the present Hilbert-space setting.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22F](../../22f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
