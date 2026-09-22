<h1 id="8b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Suppose $\mathbf v=\alpha\mathbf e_1+\beta\mathbf e_2$. Applying $M-\lambda_2I$ would give $\mathbf e_2=\alpha(\lambda_1-\lambda_2)\mathbf e_1$, contradicting [linear independence](../../../../../../linear-independence.md) of the two [eigenvectors](../../../../../../eigenvector.md). Therefore the [generalized eigenvector](../../../../../../generalized-eigenvector.md) $\mathbf v$ lies outside their span and $(\mathbf e_1,\mathbf e_2,\mathbf v)$ is a [basis](../../../../../../basis.md). Write $\mathbf x=a\mathbf e_1+b\mathbf e_2+d\mathbf v$. Since $M\mathbf v=\lambda_2\mathbf v+\mathbf e_2$, the [linear system of ordinary differential equations](../../../../../../linear-system-of-differential-equations.md) gives

$$
\dot a=\lambda_1a,\qquad\dot d=\lambda_2d,\qquad\dot b=\lambda_2b+d.
$$

Solving these equations gives $a=A_1e^{\lambda_1t}$, $d=A_3e^{\lambda_2t}$ and $b=(A_2+A_3t)e^{\lambda_2t}$. Thus

$$
\boxed{\mathbf x(t)=A_1e^{\lambda_1t}\mathbf e_1+e^{\lambda_2t}\left[A_2\mathbf e_2+A_3(\mathbf v+t\mathbf e_2)\right].}
$$

The [length-two Jordan chain solution](../../../../../../length-two-jordan-chain-solution.md) for the [Jordan chain](../../../../../../jordan-chain.md) $(\mathbf e_2,\mathbf v)$ produces the $t e^{\lambda_2t}$ mode. The three arbitrary constants span all initial data, so this is the full general solution.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [8B](../../8b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
