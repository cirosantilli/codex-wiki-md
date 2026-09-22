<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [simple module](../../../../irreducible-module.md) is nonzero and has no [submodules](../../../../submodule.md) other than zero and itself. A [semisimple module](../../../../semisimple-module.md) is a [direct sum](../../../../direct-sum.md) of simple [submodules](../../../../submodule.md); the zero [module](../../../../module-mathematics.md) is allowed as the empty sum.

For (1)$\Rightarrow$(2), argue by [dimension](../../../../dimension-vector-space.md). Choose a minimal nonzero [submodule](../../../../submodule.md) $S$, which is simple, and split $V=S\oplus C$ using (1). The property passes to $C$: for $U\subseteq C$, write $V=U\oplus D$; then $C=U\oplus(C\cap D)$. Apply induction to $C$ and append $S$. The zero-dimensional case starts the induction. The implication (2)$\Rightarrow$(3) is immediate. For (3)$\Rightarrow$(2), repeatedly append a simple [submodule](../../../../submodule.md) not contained in the sum already chosen. Its intersection with that sum is zero by simplicity. [Dimension](../../../../dimension-vector-space.md) strictly increases, so after finitely many steps their [direct sum](../../../../direct-sum.md) is $V$.

For (2)$\Rightarrow$(1), write $V=\bigoplus_iS_i$ and fix $U$. Choose a sum $C$ of a maximal subset of these $S_i$ whose sum is disjoint from $U$. If $U+C\ne V$, some $S_j$ is not contained in $U+C$, so simplicity gives $S_j\cap(U+C)=0$. Then $C+S_j$ is a larger [direct sum](../../../../direct-sum.md) still disjoint from $U$, a contradiction. Hence $V=U\oplus C$.

Condition (1) implies (1\*). Conversely suppose (1\*) and let $W$ be the sum of all simple [submodules](../../../../submodule.md). If $W\ne V$, finite [dimension](../../../../dimension-vector-space.md) supplies a maximal proper [submodule](../../../../submodule.md) $M$ containing $W$. By (1\*), $V=M\oplus C$. Projection to the simple quotient $V/M$ identifies the nonzero complement $C$ with a [simple module](../../../../irreducible-module.md). Thus $C\subseteq W\subseteq M$, contradicting the [direct sum](../../../../direct-sum.md). Consequently $W=V$, which is (3). This proves **all four conditions are equivalent**.

For the concrete complement, $x^2=x$. [Orthogonal idempotents](../../../../orthogonal-idempotent.md) $x$ and $1-x$ give $A=Ax\oplus A(1-x)$: the sum follows from $1=x+(1-x)$, and right multiplication by $x$ shows their intersection is zero. In explicit [matrix](../../../../matrix.md) form,

$$
\boxed{U=\left\{\begin{pmatrix}a&\lambda a\\b&\lambda b\end{pmatrix}:a,b\in K\right\},\qquad C=\left\{\begin{pmatrix}0&c\\0&d\end{pmatrix}:c,d\in K\right\}=A(1-x).}
$$

The decomposition of $\begin{pmatrix}a&b\\c&d\end{pmatrix}$ uses second-column remainders $b-\lambda a,d-\lambda c$ in $C$.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the algebra course of the University of Oxford](../../../split.md)
5. [Algebra course of the University of Oxford](../../../../algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
