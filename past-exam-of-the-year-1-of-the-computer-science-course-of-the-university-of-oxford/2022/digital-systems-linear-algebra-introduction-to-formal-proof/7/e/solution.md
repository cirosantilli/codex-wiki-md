<h1 id="7/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Only $\psi$ requires a [natural deduction](../../../../../natural-deduction.md) proof. Assume $h:(A\lor B)\to C$. Within that assumption, temporarily assume $a:A$. By disjunction introduction, obtain $A\lor B$; applying $h$ by the [implication elimination rule](../../../../../implication-elimination-rule.md) gives $C$. Discharge $a$ by the [implication introduction rule](../../../../../implication-introduction-rule.md) to derive $A\to C$. Disjunction introduction now gives $(A\to C)\lor(B\to C)$. Finally discharge $h$ by the [implication introduction rule](../../../../../implication-introduction-rule.md):

$$
\frac{
\begin{array}{c}
[(A\lor B)\to C]^1\qquad
\dfrac{[A]^2}{A\lor B}\ {\lor I_L}\\[3pt]
\dfrac{(A\lor B)\to C\qquad A\lor B}{C}\ {\to E}\\[5pt]
\dfrac{C}{A\to C}\ {\to I}^{,2}\\[5pt]
\dfrac{A\to C}{(A\to C)\lor(B\to C)}\ {\lor I_L}
\end{array}}
{\bigl((A\lor B)\to C\bigr)\to\bigl((A\to C)\lor(B\to C)\bigr)}\ {\to I}^{,1}.
$$

All temporary assumptions are discharged. No classical rule is needed; the same proof works in [Intuitionistic propositional logic](../../../../../intuitionistic-propositional-logic.md). The false [propositional formula](../../../../../propositional-formula.md) $\varphi$ has no proof in this sound [natural deduction](../../../../../natural-deduction.md) system.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
