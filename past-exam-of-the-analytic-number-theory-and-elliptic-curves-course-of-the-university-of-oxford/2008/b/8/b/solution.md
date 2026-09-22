<h1 id="b/8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For [prime-power contraction in a formal group](../../../../../prime-power-contraction-in-a-formal-group.md), a one-dimensional [formal group](../../../../../formal-group-law.md) over $R$ has $F(X,Y)=X+Y+$ terms of total degree at least two with [coefficients](../../../../../coefficient.md) in $R$. Induction under composition therefore gives

$$
[p](X)=pX+\sum_{j\ge2}c_jX^j,\qquad c_j\in R.
$$

For $|x|<1$ this converges and the non-Archimedean inequality gives $|[p](x)|\le\max(|p||x|,|x|^2)$. The [residue](../../../../../residue.md) [characteristic](../../../../../characteristic-of-a-field.md) implies $|p|<1$; in equal [characteristic](../../../../../characteristic-of-a-field.md) $p$ the linear [coefficient](../../../../../coefficient.md) is zero, which only improves the bound.

Let $x_n=[p^n](x)$, so $x_{n+1}=[p](x_n)$. If $x=0$ there is nothing to prove. Otherwise put $\rho=\max(|p|,|x|)<1$. Inductively $|x_n|\le|x|$, and then $|x_{n+1}|\le\rho|x_n|$. Thus

$$
\boxed{|[p^n](x)|\le\rho^n|x|\longrightarrow0.}
$$

Completeness ensures convergence of the formal-series evaluations. The contraction argument in fact does not need the extra discreteness assumption.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
