<h1 id="17b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Q=Q_{n+1}$. By [polynomial division](../../../../../../polynomial-division.md), every $q\in\mathcal P_{n+1+k}$ has a unique decomposition

$$
q=Qs+r,
\qquad s\in\mathcal P_k,\qquad r\in\mathcal P_n.
$$

Every node is a zero of $Q$, so $I_n(Qs)=0$. The assumed degree-$n$ exactness also gives $I_n(r)=I(r)$. Hence

$$
I_n(q)=I(r),
\qquad
I(q)=I(Qs)+I(r).
$$

Therefore $I_n(q)=I(q)$ for every $q\in\mathcal P_{n+1+k}$ if and only if

$$
I(Qs)=\langle Q,s\rangle=0
$$

for every $s\in\mathcal P_k$. This proves the [nodal-polynomial criterion for quadrature exactness](../../../../../../nodal-polynomial-criterion-for-quadrature-exactness.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17B](../../17b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
