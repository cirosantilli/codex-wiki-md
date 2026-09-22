<h1 id="22f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume $u(0)=0$. Applying midpoint preservation to $2v$ and $0$ gives

$$
u(v)=\frac{u(2v)+u(0)}2=\frac12u(2v),
$$

so $u(2v)=2u(v)$. Consequently,

$$
u(v+w)
=u\left(2\frac{v+w}{2}\right)
=2u\left(\frac{v+w}{2}\right)
=u(v)+u(w).
$$

Thus $u$ is additive. It follows successively that

$$
u(nv)=nu(v)
\quad(n\in\mathbb Z),
\qquad
u(qv)=qu(v)
\quad(q\in\mathbb Q).
$$

An isometry is continuous. For any $\lambda\in\mathbb R$, choose rationals $q_j\to\lambda$. Then

$$
u(\lambda v)
=\lim_{j\to\infty}u(q_jv)
=\lim_{j\to\infty}q_ju(v)
=\lambda u(v).
$$

Together with additivity, this proves that $u$ is real-linear. Hence the origin-fixing case of the [Mazur-Ulam theorem](../../../../../../mazur-ulam-theorem.md) gives

$$
\boxed{u(av+bw)=au(v)+bu(w)}
$$

for all $a,b\in\mathbb R$ and $v,w\in V$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22F](../../22f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
