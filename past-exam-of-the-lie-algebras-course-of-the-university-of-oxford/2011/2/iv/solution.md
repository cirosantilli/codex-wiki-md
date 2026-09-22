<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

On a monomial $X^aY^b$, direct [differentiation](../../../../differentiation.md) gives

$$
E(X^aY^b)=bX^{a+1}Y^{b-1},\quad
F(X^aY^b)=aX^{a-1}Y^{b+1},\quad
H(X^aY^b)=(a-b)X^aY^b.
$$

For example $(EF-FE)(X^aY^b)=[a(b+1)-b(a+1)]X^aY^b=(a-b)X^aY^b$. The same calculation with $H$ gives

$$
[H,E]=2E,\qquad[H,F]=-2F,\qquad[E,F]=H.
$$

These are exactly the brackets of $h,e,f$, so the [linear map](../../../../linear-map.md) $\rho$ respects every bracket and is a [Lie algebra representation](../../../../lie-algebra-representation.md).

For $m\ge0$, let $W_m$ be the space of [homogeneous polynomials](../../../../homogeneous-polynomial.md) of [total degree](../../../../total-degree-of-a-polynomial.md) $m$. Each operator preserves [total degree](../../../../total-degree-of-a-polynomial.md). Every [polynomial](../../../../polynomial-split.md) is a finite sum of homogeneous polynomials, so

$$
W=\bigoplus_{m=0}^{\infty}W_m.
$$

In $W_m$, the monomials $v_j=X^{m-j}Y^j$ have distinct weights $m-2j$ and exactly the actions described in part (i). To see simplicity directly, a nonzero [invariant subspace](../../../../invariant-subspace.md) is invariant under $H$ and hence contains one of its weight components: [polynomial interpolation](../../../../polynomial-interpolation.md) in $H$ projects onto each of its distinct eigenspaces. Starting with a nonzero multiple of $v_j$, repeated application of $E$ reaches $v_0$, and repeated application of $F$ then reaches all $v_j$. All coefficients used are nonzero in characteristic zero. Therefore $W_m$ is simple and isomorphic to $L_m$.

Thus

$$
\boxed{\mathbb C[X,Y]=\bigoplus_{m\ge0}\operatorname{span}\{X^m,X^{m-1}Y,\ldots,Y^m\}
\cong\bigoplus_{m\ge0}L_m.}
$$

This is an algebraic [direct sum](../../../../direct-sum.md), not an infinite product or completion. Its simple submodules are precisely the $W_m$: they are pairwise nonisomorphic and each occurs once, so projection onto homogeneous degrees and [Schur's lemma](../../../../schur-s-lemma.md) exclude diagonal copies between distinct degrees. Complete reducibility here follows from the explicit decomposition, rather than applying a finite-dimensional theorem directly to the infinite-dimensional $W$.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Lie algebras course of the University of Oxford](../../../split.md)
5. [Lie algebras course of the University of Oxford](../../../../lie-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
