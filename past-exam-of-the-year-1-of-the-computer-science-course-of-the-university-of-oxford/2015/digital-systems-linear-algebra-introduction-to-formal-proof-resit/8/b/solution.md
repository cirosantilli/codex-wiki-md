<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $H=\forall x\forall y(S(x,y)\lor\neg S(x,y))$ and abbreviate

$$
B(b)=\forall p\,((S(b,p)\to\neg S(p,p))\land(\neg S(p,p)\to S(b,p))).
$$

Assume $\exists b\,B(b)$ and eliminate the [existential quantifier](../../../../../existential-quantification.md) using a fresh [eigenvariable](../../../../../eigenvariable.md) $u$. Inside that [subproof](../../../../../subproof.md), specialize $B(u)$ at $p=u$. Write $s=S(u,u)$. The premise $H$ supplies $s\lor\neg s$, so a [disjunction elimination rule](../../../../../disjunction-elimination-rule.md) finishes the contradiction:

$$
\begin{array}{rll}
1&H&\text{premise}\\
2&[\exists b\,B(b)]^a&\text{assumption}\\
3&\quad[B(u)]^b&\text{fresh witness assumption}\\
4&\qquad(s\to\neg s)\land(\neg s\to s)&\forall E\ 3\ (p=u)\\
5&\qquad s\to\neg s&\land E\ 4\\
6&\qquad\neg s\to s&\land E\ 4\\
7&\qquad s\lor\neg s&\forall E\text{ twice on }1\ (x=y=u)\\
8&\qquad[s]^c&\text{assumption}\\
9&\qquad\quad\neg s&\to E\ 8,5\\
10&\qquad\quad\bot&\neg E\ 8,9\\
11&\qquad[\neg s]^d&\text{assumption}\\
12&\qquad\quad s&\to E\ 11,6\\
13&\qquad\quad\bot&\neg E\ 12,11\\
14&\qquad\bot&\lor E\ 7,(8\text{--}10),(11\text{--}13)\\
15&\quad\bot&\exists E\ 2,(3\text{--}14)\\
16&\neg\exists b\,B(b)&\neg I\ (2\text{--}15).
\end{array}
$$

Line 7 abbreviates two consecutive [universal quantifier elimination rule](../../../../../universal-quantifier-elimination-rule.md) applications; no new rule is used. The fresh witness $u$ is absent from $H$, the assumed existential statement and the exported $\bot$, so the [existential quantifier elimination rule](../../../../../existential-quantifier-elimination-rule.md) satisfies its [eigenvariable condition](../../../../../eigenvariable-condition.md). This is the self-application behind the [barber paradox](../../../../../barber-paradox.md), written entirely with the supplied rules.

$$
\boxed{H\vdash\neg\exists b\,\forall p\,((S(b,p)\to\neg S(p,p))\land(\neg S(p,p)\to S(b,p))).}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
