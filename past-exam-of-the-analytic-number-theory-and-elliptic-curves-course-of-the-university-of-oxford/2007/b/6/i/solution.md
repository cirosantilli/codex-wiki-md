<h1 id="b/6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

If $p=0$ as an element of $K$, the stated lower bound is zero and is immediate. Otherwise set $\rho_1=|p|^{1/(p-1)}$. The supplied [formal group](../../../../../formal-group-law.md) expansion has $g(0)=0$, because $[p](0)=0$. For $z\in\mathcal M$, the non-Archimedean estimates give

$$
|f(z)|=|z|,\qquad |g(z^p)|\le|z|^p,\qquad
|[p](z)|\le\max\{|p||z|,|z|^p\}.
$$

If $0<|z|<\rho_1$, then $|z|^p<|p||z|$, so the two terms cannot cancel and $|[p](z)|=|p||z|>0$. The same strict inequality persists under iteration, so no such $z$ can have finite $p$-power order. Every nonzero $p$-power torsion point therefore satisfies $|z|\ge\rho_1$.

For a point of order $p$, $[p](z)=0$ itself forces $|p||z|\le|z|^p$, proving the bound for $n=1$. For $n\ge2$, put $w=[p](z)$, of order $p^{n-1}$. Since $|z|\ge\rho_1$, the preceding maximum is $|z|^p$. By induction,

$$
|z|^p\ge|w|\ge|p|^{1/(p^{n-1}-p^{n-2})}.
$$

This proves the [formal torsion radius for prime power order](../../../../../formal-torsion-radius-for-prime-power-order.md). Taking the positive $p$th root gives

$$
\boxed{|z|\ge|p|^{1/(p^n-p^{n-1})}.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
