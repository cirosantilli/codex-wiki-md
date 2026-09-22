<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

Both candidate sets contain zero. The [sum of subspaces](../../../../../sum-of-vector-subspaces.md) is closed under [linear combinations](../../../../../linear-combination.md) because $a(u_1+w_1)+b(u_2+w_2)=(au_1+bu_2)+(aw_1+bw_2)$, with the two terms in $U$ and $W$. The intersection is closed because any [linear combination](../../../../../linear-combination.md) of vectors lying in both subspaces still lies in both. Thus each is a [vector subspace](../../../../../vector-subspace.md).

Take a [basis](../../../../../basis.md) $s_1,\ldots,s_r$ of the intersection, extend it by $u_1,\ldots,u_a$ to a [basis](../../../../../basis.md) of $U$, and by $w_1,\ldots,w_b$ to a [basis](../../../../../basis.md) of $W$. The combined list $s,u,w$ spans $U+W$. To prove independence, a zero combination makes the $u$ combination equal a vector in both $U$ and $W$, so it is a combination of the $s$'s. Independence of the [basis](../../../../../basis.md) of $U$ makes all $u$ coefficients zero; independence of the [basis](../../../../../basis.md) of $W$ then makes all remaining coefficients zero. Hence $\dim(U+W)=r+a+b$, giving the [dimension formula for a sum of subspaces](../../../../../dimension-formula-for-a-sum-of-subspaces.md)

$$
\boxed{\dim U+\dim W=\dim(U+W)+\dim(U\cap W).}
$$

For the concrete kernels, the equations $Ax=0$ give

$$
x=\left(\frac{5s-5t}{3},\frac{-s+7t}{3},s,t\right).
$$

Applying the two rows of $B$ to this expression gives $4(s-t)$ and $5(s-t)/3$. Thus the intersection has [basis](../../../../../basis.md) $v_0=(0,2,1,1)$. Choose $v_1=(5,-1,3,0)$ in $U$ and $v_2=(-4,-2,1,0)$ in $W$. Then

$$
\boxed{\mathcal B_{U\cap W}=(v_0),\quad\mathcal B_U=(v_0,v_1),\quad
\mathcal B_{U+W}=(v_0,v_1,v_2).}
$$

Indeed $U$ has dimension two because $A$ has rank two, and $v_0,v_1$ are independent. Likewise $W$ has dimension two and $v_0,v_2$ are independent, so the last list spans the sum. Its first three coordinates have determinant $-48$, confirming independence and dimension three.

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
