<h1 id="8/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose fresh arbitrary [eigenvariables](../../../../../../eigenvariable.md) $u,v$. Under $u=v$, use the [equality elimination rule](../../../../../../equality-elimination-rule.md) to transport $P(u)$ to $P(v)$. For the reverse direction, first derive $v=u$ by the symmetry derivation above. In full [natural deduction](../../../../../../natural-deduction.md) form:

$$
\begin{array}{rll}
1&[u=v]^a&\text{assumption}\\
2&\quad[P(u)]^b&\text{assumption}\\
3&\qquad P(v)&=E\ 1,2\\
4&\quad P(u)\to P(v)&\to I\ (2\text{--}3)\\
5&\quad u=u&=I\\
6&\quad v=u&=E\ 1,5\quad(\phi(w)\equiv w=u)\\
7&\quad[P(v)]^c&\text{assumption}\\
8&\qquad P(u)&=E\ 6,7\\
9&\quad P(v)\to P(u)&\to I\ (7\text{--}8)\\
10&\quad(P(u)\to P(v))\land(P(v)\to P(u))&\land I\ 4,9\\
11&u=v\to((P(u)\to P(v))\land(P(v)\to P(u)))&\to I\ (1\text{--}10)\\
12&\forall y\,(u=y\to((P(u)\to P(y))\land(P(y)\to P(u))))&\forall I\ 11\\
13&\forall x\forall y\,(x=y\to((P(x)\to P(y))\land(P(y)\to P(x))))&\forall I\ 12.
\end{array}
$$

All [temporary assumptions](../../../../../../temporary-assumption.md) are discharged before either [universal quantifier introduction rule](../../../../../../universal-quantifier-introduction-rule.md) application, so both [eigenvariable conditions](../../../../../../eigenvariable-condition.md) hold. No premises remain:

$$
\boxed{\vdash\forall x\forall y\,(x=y\to((P(x)\to P(y))\land(P(y)\to P(x)))).}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [8](../../../8.md)
4. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
