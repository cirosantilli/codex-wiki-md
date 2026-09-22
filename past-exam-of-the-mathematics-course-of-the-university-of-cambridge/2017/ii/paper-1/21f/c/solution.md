<h1 id="21f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $Y=X^{**}$, which is a [Banach space](../../../../../../banach-space-split.md) by the completeness of the dual just proved. The [canonical embedding into the bidual](../../../../../../canonical-embedding-into-the-bidual.md) is

$$
\Phi(x)(f)=f(x),\qquad f\in X^*.
$$

For fixed $x$ this is a bounded [linear functional](../../../../../../linear-functional.md) on $X^*$, since $|f(x)|\le\|f\|\|x\|$, and $\Phi$ is linear in $x$. This gives $\|\Phi(x)\|\le\|x\|$. For $x\ne0$, the norming functional from the [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) has $\|f\|=1$ and $f(x)=\|x\|$, giving the reverse inequality. At zero equality is immediate. Thus

$$
\boxed{\|\Phi(x)\|=\|x\|\text{ for all }x\in X}.
$$

In particular $\Phi$ is injective and isometric. If a dense isometric embedding is wanted, rather than merely the stated embedding, take the [norm](../../../../../../norm.md) closure of $\Phi(X)$ in $X^{**}$; a closed subspace of a [Banach space](../../../../../../banach-space-split.md) is complete and supplies a [completion of a normed space](../../../../../../completion-of-a-normed-space.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [21F](../../21f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
