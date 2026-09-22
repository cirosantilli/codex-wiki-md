<h1 id="8f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An endomorphism $\alpha$ is a projection onto its image precisely when it is the identity on $\operatorname{im}\alpha$ and kills a complementary subspace. If $\alpha^2=\alpha$, then

$$
\alpha(\alpha v)=\alpha v,
$$

so $\alpha$ is the identity on its image. Moreover,

$$
v=\alpha v+(v-\alpha v),
\qquad
\alpha(v-\alpha v)=0,
$$

and $\operatorname{im}\alpha\cap\ker\alpha=\{0\}$. Hence

$$
V=\operatorname{im}\alpha\oplus\ker\alpha,
$$

and $\alpha$ is the projection onto its image along its kernel. Conversely, every projection is the identity after one application, so applying it twice has the same effect: $\alpha^2=\alpha$.

Statement (i) is **false**. On a two-dimensional vector space, take the nonzero nilpotent endomorphism

$$
\alpha=
\begin{pmatrix}
0&1\\
0&0
\end{pmatrix}.
$$

Then $\alpha^2=\alpha^3=0$, but $\alpha^2\ne\alpha$, so $\alpha$ is not [idempotent](../../../../../../idempotent.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [8F](../../8f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
