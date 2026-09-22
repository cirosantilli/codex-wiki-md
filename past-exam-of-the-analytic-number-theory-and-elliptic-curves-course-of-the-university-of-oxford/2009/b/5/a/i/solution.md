<h1 id="b/5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $U(T)=F_X(0,T)$. The [formal group](../../../../../../formal-group-law.md) identity $F(X,0)=X$ gives $U(0)=1$, so $U$ is a [unit in a ring](../../../../../../unit-in-a-ring.md) in $R[[T]]$, even if $R$ has [zero divisors](../../../../../../zero-divisor.md).

A differential $h(T)dT$ is invariant under formal translation if

$$
h(F(X,T))F_X(X,T)=h(X)
$$

as an identity of [formal power series](../../../../../../formal-power-series.md). Setting $X=0$ gives $h(T)U(T)=h(0)$. Consequently every [invariant differential of a formal group law](../../../../../../invariant-differential-of-a-formal-group-law.md), if it exists, must have the form $h(0)U(T)^{-1}dT$. In particular there can be only one with constant coefficient one.

Existence follows directly from associativity. Differentiate

$$
F(Z,F(X,T))=F(F(Z,X),T)
$$

with respect to $Z$ at zero, obtaining

$$
U(F(X,T))=F_X(X,T)U(X).
$$

Every displayed $U$ is a [unit in a ring](../../../../../../unit-in-a-ring.md), so

$$
U(F(X,T))^{-1}F_X(X,T)=U(X)^{-1}.
$$

This is precisely invariance of $U(T)^{-1}dT$. Thus

$$
\boxed{\omega=F_X(0,T)^{-1}dT,\qquad
\{\text{invariant differentials}\}=R\omega.}
$$

Normalization means its constant coefficient is one. This proves both existence and uniqueness over an arbitrary [commutative ring](../../../../../../commutative-ring.md), without division by any [integer](../../../../../../integer-split.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../../split.md)
7. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
