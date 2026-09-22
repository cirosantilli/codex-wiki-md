<h1 id="9e/solution">Solution</h1>

↑ **Parent:** [9E](../9e.md)

The external [direct sum of vector spaces](../../../../../direct-sum.md) consists of pairs $(v_1,v_2)$ with componentwise operations. For subspaces of one ambient space, the [sum of vector subspaces](../../../../../sum-of-vector-subspaces.md) is $V_1+V_2=\{v_1+v_2:v_i\in V_i\}$. The addition map from the external direct sum onto this subspace is surjective, with kernel $\{(w,-w):w\in V_1\cap V_2\}$. This kernel is isomorphic to the intersection. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md), together with $\dim(V_1\oplus V_2)=\dim V_1+\dim V_2$, proves the [dimension formula for a sum of subspaces](../../../../../dimension-formula-for-a-sum-of-subspaces.md).

For the supplied bases, solving for annihilating linear forms gives

$$
V_1=\{x:x_1+x_2-x_3+x_4=0\},\qquad
V_2=\{x:2x_1-3x_3+x_4=0\}.
$$

Each [basis](../../../../../basis.md) has rank three, so these hyperplanes are the whole subspaces. The two independent equations make the intersection two-dimensional. Imposing the requested zero components yields

$$
\boxed{v_1=(0,-2,1,3),\qquad v_2=(-2,0,-1,1).}
$$

Both satisfy the two equations and are independent, since their first components differ while $v_1\ne0$. Hence they form the required [basis](../../../../../basis.md).

## ↑ Ancestors (10)

1. [9E](../9e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
