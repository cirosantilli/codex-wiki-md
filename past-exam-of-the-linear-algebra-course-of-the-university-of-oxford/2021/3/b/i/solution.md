<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

For the given [nondegenerate bilinear form](../../../../../nondegenerate-bilinear-form.md), define the [linear map](../../../../../linear-map.md)

$$
\Phi:V\longrightarrow V',\qquad \Phi(v)(u)=(u,v).
$$

By part (a), $\Phi$ is a [linear isomorphism](../../../../../linear-isomorphism.md). The paper's [bilinear orthogonal complement](../../../../../orthogonal-complement-for-a-bilinear-form.md) uses $U$ in the first argument; with this convention,

$$
U^\perp=\Phi^{-1}(U^0),\qquad
U^0=\{f\in V':f(u)=0\text{ for every }u\in U\}.
$$

Here $U^0$ is the [annihilator of a vector subspace](../../../../../annihilator-of-a-vector-subspace.md) $U$. Since $\Phi$ is a [linear isomorphism](../../../../../linear-isomorphism.md), its [restriction](../../../../../restriction-mathematics.md) gives a [linear isomorphism](../../../../../linear-isomorphism.md) $U^\perp\to U^0$.

For completeness, choose a [basis](../../../../../basis.md) $u_1,\ldots,u_k$ of $U$ and extend it to a [basis](../../../../../basis.md) $u_1,\ldots,u_n$ of $V$. In its [dual basis](../../../../../dual-basis.md) $u_1^*,\ldots,u_n^*$, a [linear functional](../../../../../linear-functional.md) vanishes on $U$ exactly when its first $k$ [coefficients](../../../../../coefficient.md) are zero. Therefore

$$
U^0=\operatorname{span}\{u_{k+1}^*,\ldots,u_n^*\},\qquad \dim U^0=n-k.
$$

Consequently

$$
\boxed{\dim U^\perp=\dim U^0=\dim V-\dim U,\qquad
\dim U+\dim U^\perp=\dim V.}
$$

The argument includes $U=0$ and $U=V$, and requires no symmetry assumption on the [bilinear form](../../../../../bilinear-form-split.md).

## ↑ Ancestors (13)

1. [i](../i.md)
2. [b](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
