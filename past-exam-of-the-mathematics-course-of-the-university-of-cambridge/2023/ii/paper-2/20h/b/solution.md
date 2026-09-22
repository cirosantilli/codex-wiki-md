<h1 id="20h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\theta=\sqrt[3]{3}$. The given ring of integers has integral basis $1,\theta,\theta^2$. The discriminant of the power basis, equivalently of $T^3-3$, is

$$
d_K=-27\cdot3^2=-243.
$$

The field has signature $(1,1)$: one real embedding and one conjugate pair of complex embeddings. The [Minkowski bound for ideal classes](../../../../../../minkowski-s-bound.md) is therefore

$$
\left(\frac4\pi\right)\frac{3!}{3^3}\sqrt{243}
=\frac{8\sqrt3}{\pi}<5.
$$

Every ideal class consequently has an integral representative of norm at most four.

It remains to inspect prime ideals above $2$ and $3$. Modulo $2$,

$$
T^3-3\equiv T^3+1
=(T+1)(T^2+T+1).
$$

The [Dedekind factorization theorem](../../../../../../dedekind-factorization-theorem.md) gives

$$
(2)=\mathfrak p_2\mathfrak q_2,
$$

where

$$
\mathfrak p_2=(2,\theta-1),\quad N(\mathfrak p_2)=2,
\qquad
\mathfrak q_2=(2,\theta^2+\theta+1),\quad N(\mathfrak q_2)=4.
$$

But

$$
N_{K/\mathbb Q}(\theta-1)=3-1=2,
$$

so the principal ideal $(\theta-1)$ is contained in $\mathfrak p_2$ and has the same norm; hence

$$
\mathfrak p_2=(\theta-1).
$$

Also

$$
(\theta-1)(\theta^2+\theta+1)=\theta^3-1=2,
$$

so

$$
\mathfrak q_2=(\theta^2+\theta+1).
$$

Both primes above $2$ are principal.

Finally,

$$
(\theta)^3=(3),
\qquad
N((\theta))=|N_{K/\mathbb Q}(\theta)|=3.
$$

Thus the unique prime above $3$ is the principal ideal $(\theta)$. By [unique factorization of ideals in a number field](../../../../../../unique-factorization-of-ideals-in-a-number-field.md), every integral ideal of norm at most four is built from these principal prime ideals. Every ideal class is therefore trivial, and the [Class group of Q of cube root of three](../../../../../../class-group-of-q-of-cube-root-of-three.md) is

$$
\boxed{\operatorname{Cl}\bigl(\mathbb Q(\sqrt[3]{3})\bigr)=1.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20H](../../20h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
