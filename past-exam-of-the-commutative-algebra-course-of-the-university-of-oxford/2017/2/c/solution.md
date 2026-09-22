<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $n\geq1$ and suppose, for a contradiction, that $I^n=I^{n+1}$. Set $M=I^n$. Since $R$ is a [Noetherian ring](../../../../noetherian-ring.md), this [ideal](../../../../ideal.md) is a [finitely generated module](../../../../finitely-generated-module.md), say $M=(u_1,\ldots,u_r)$. It is nonzero: if $0\ne a\in I$, then $a^n\ne0$ because $R$ is an [integral domain](../../../../integral-domain.md).

The equality $M=IM$ allows us to write

$$
u_i=\sum_{j=1}^r a_{ij}u_j,\qquad a_{ij}\in I.
$$

Let $A=(a_{ij})$ and $B=\operatorname{Id}_r-A$. Then $B(u_1,\ldots,u_r)^{\mathsf T}=0$. The [adjugate matrix](../../../../adjugate-matrix.md) identity $\operatorname{adj}(B)B=(\det B)\operatorname{Id}_r$ implies that $\det B$ annihilates every $u_i$. In the [determinant](../../../../determinant.md) expansion of $\operatorname{Id}_r-A$, the constant term is $1$ and every other term contains an entry of $A$, so

$$
\det B=1-b\quad\text{for some }b\in I.
$$

This is the [determinant trick](../../../../determinant-trick.md). Since some $u_i\ne0$, [multiplicative cancellation in an integral domain](../../../../multiplicative-cancellation-in-an-integral-domain.md) gives $1-b=0$. But then $1=b\in I$, contradicting $I\ne R$. We have proved the [strict descent of powers of a nonzero proper ideal in a Noetherian domain](../../../../strict-descent-of-powers-of-a-nonzero-proper-ideal-in-a-noetherian-domain.md):

$$
\boxed{I\supsetneq I^2\supsetneq I^3\supsetneq\cdots.}
$$

All these [powers of an ideal](../../../../powers-of-an-ideal.md) have the same [radical of an ideal](../../../../radical-of-an-ideal.md). Indeed, $I^n\subseteq I$ gives $\sqrt{I^n}\subseteq\sqrt I$. Conversely, if $x^m\in I$, then $x^{mn}\in I^n$, so $x\in\sqrt{I^n}$. Thus

$$
\boxed{\sqrt{I^n}=\sqrt I\quad(n\geq1),}
$$

and $J=I,I^2,I^3,\ldots$ gives infinitely many distinct [ideals](../../../../ideal.md) with the prescribed [radical of an ideal](../../../../radical-of-an-ideal.md). If the convention $0\in\mathbb N$ is used, the additional inequality $I^0=R\ne I$ follows immediately from properness.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the commutative algebra course of the University of Oxford](../../../split.md)
5. [Commutative algebra course of the University of Oxford](../../../../commutative-algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
