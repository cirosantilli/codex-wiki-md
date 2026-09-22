<h1 id="8/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose $v$ fresh. Here [double-negation elimination](../../../../../../double-negation-elimination.md) is necessary to turn the [negation](../../../../../../negation.md) of a possible counterexample into the positive statement:

$$
\begin{array}{rll}
1&\neg\exists x\,\neg R(x)&\text{premise}\\
2&\vert\ \neg R(v)&\text{assumption; }v\text{ fresh}\\
3&\vert\ \exists x\,\neg R(x)&\exists\text{-intro }2\\
4&\vert\ \bot&\neg\text{-elim }3,1\\
5&\neg\neg R(v)&\neg\text{-intro }2\text{--}4\\
6&R(v)&\neg\neg\text{-elim }5\\
7&\forall y\,R(y)&\forall\text{-intro }6
\end{array}
$$

The remaining context at line 7 contains no free $v$. The [universal quantifier introduction rule](../../../../../../universal-quantifier-introduction-rule.md) therefore gives

$$
\boxed{\neg\exists x\,\neg R(x)\ \vdash\ \forall y\,R(y).}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
