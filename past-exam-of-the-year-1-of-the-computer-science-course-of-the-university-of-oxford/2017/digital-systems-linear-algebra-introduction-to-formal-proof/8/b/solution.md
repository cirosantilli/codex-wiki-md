<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The two proofs differ in whether [existential elimination](../../../../../existential-quantifier-elimination-rule.md) is outside or inside [negation introduction](../../../../../negation-introduction-rule.md). For the first proof, choose fresh $a$, derive the negation inside the witness subproof, and then discharge the witness:

$$
\begin{array}{rll}
1&\exists x\,\neg P(x)&\text{premise}\\
2&\quad\neg P(a)&\text{fresh witness assumption}\\
3&\qquad\forall y\,P(y)&\text{assumption}\\
4&\qquad P(a)&\forall E\ 3\\
5&\qquad\bot&\neg E\ 4,2\\
6&\quad\neg\forall y\,P(y)&\neg I\ 3\text{--}5\\
7&\neg\forall y\,P(y)&\exists E\ 1,2\text{--}6
\end{array}
$$

The conclusion at line 6 contains no free $a$. For the second proof, open the universal assumption first, eliminate the existential to derive falsity, and then discharge the universal assumption:

$$
\begin{array}{rll}
1&\exists x\,\neg P(x)&\text{premise}\\
2&\quad\forall y\,P(y)&\text{assumption}\\
3&\qquad\neg P(a)&\text{fresh witness assumption}\\
4&\qquad P(a)&\forall E\ 2\\
5&\qquad\bot&\neg E\ 4,3\\
6&\quad\bot&\exists E\ 1,3\text{--}5\\
7&\neg\forall y\,P(y)&\neg I\ 2\text{--}6
\end{array}
$$

At line 6 of the second proof, neither the exported conclusion $\bot$ nor the other open assumptions contains $a$ free, satisfying the [eigenvariable condition](../../../../../eigenvariable-condition.md). Neither proof needs RAA or [double-negation elimination](../../../../../double-negation-elimination.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
