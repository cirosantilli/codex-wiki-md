<h1 id="f/f2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the variables as $(u,v)\in\mathbb R^n\times\mathbb R^k$, with $a=(u_0,v_0)$. The hypothesis makes $D_uf(a)$ invertible. The [implicit function theorem](../../../../../implicit-function-theorem.md) supplies neighbourhoods $U,V$ of $u_0,v_0$ and a unique [smooth map](../../../../../smooth-map-between-manifolds.md) $\phi:V\to U$ such that

$$
\boxed{f^{-1}(b)\cap(U\times V)=\{(\phi(v),v):v\in V\},\quad \phi(v_0)=u_0.}
$$

Its derivative is $D\phi(v_0)=-(D_uf(a))^{-1}D_vf(a)$. Thus the derivative of this parametrization has image exactly $\ker Df(a)$.

Since $h$ has a constrained maximum at $a$, differentiating $v\mapsto h(\phi(v),v)$ gives zero in every direction. Therefore $Dh(a)$ vanishes on $\ker Df(a)$. In finite-dimensional [linear algebra](../../../../../linear-algebra-split.md), $(\ker Df(a))^\perp$ is the [row space](../../../../../row-space.md) of $Df(a)$. Consequently

$$
\boxed{\nabla h(a)=\sum_{j=1}^n\lambda_j\nabla f_j(a).}
$$

The full-rank hypothesis is what permits this [Lagrange multiplier](../../../../../lagrange-multiplier.md) conclusion; it is not a consequence of constrained maximality alone at a singular constraint.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [F2](../../f2.md)
3. [F](../../../f.md)
4. [2004](../../../../2004-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
