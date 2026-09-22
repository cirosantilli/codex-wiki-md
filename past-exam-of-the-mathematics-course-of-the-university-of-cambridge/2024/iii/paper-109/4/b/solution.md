<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $v\in S^{n-1}$, orthogonally project every member of $\mathcal C_i$ onto the oriented line $\ell_v$. These projections are compact intervals. They are pairwise intersecting because the original sets are, and pairwise intersecting intervals have a common intersection. Let $m_i(v)$ be the midpoint of that common interval and let $f_i(v)$ be its signed coordinate on $\ell_v$. Compactness makes $f_i$ continuous, and reversing the orientation gives

$$
f_i(-v)=-f_i(v).
$$

Define the continuous antipodal map

$$
F:S^{n-1}\longrightarrow\mathbb R^{n-1},
\qquad
F(v)=(f_1(v)-f_n(v),\ldots,f_{n-1}(v)-f_n(v)).
$$

The [Borsuk-Ulam theorem](../../../../../../borsuk-ulam-theorem.md) gives $v$ with $F(v)=0$. Write the common value as $t$. The hyperplane

$$
H=\{x\in\mathbb R^n:x\cdot v=t\}
$$

meets every set in every $\mathcal C_i$, because $t=f_i(v)$ lies in the projection interval of each such set. Thus $H$ is the required common hyperplane transversal.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
