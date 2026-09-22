<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The premise limits every possible [existential witness](../../../../../existential-witness.md) to the objects named by $c_0,c_1$; it does not assert that these constants name distinct objects. Instantiate it at a fresh witness $v$, then apply [disjunction elimination](../../../../../disjunction-elimination-rule.md). In the first case [equality elimination rule](../../../../../equality-elimination-rule.md) transfers $R(v)$ to $R(c_0)$; in the second it transfers $R(v)$ to $R(c_1)$, contradicting the assumed [negation](../../../../../negation.md). The full [natural deduction](../../../../../natural-deduction.md) derivation is

$$
\begin{array}{rll}
1&\forall x\,(x=c_0\lor x=c_1)&\text{premise}\\
2&\vert\ \neg R(c_1)&\text{assumption}\\
3&\vert\ \vert\ \exists x\,R(x)&\text{assumption}\\
4&\vert\ \vert\ \vert\ R(v)&\text{witness assumption; }v\text{ fresh}\\
5&\vert\ \vert\ \vert\ v=c_0\lor v=c_1&\forall\text{-elim }1\\
6&\vert\ \vert\ \vert\ \vert\ v=c_0&\text{first case assumption}\\
7&\vert\ \vert\ \vert\ \vert\ R(c_0)&=\text{-elim }6,4\\
8&\vert\ \vert\ \vert\ \vert\ v=c_1&\text{second case assumption}\\
9&\vert\ \vert\ \vert\ \vert\ R(c_1)&=\text{-elim }8,4\\
10&\vert\ \vert\ \vert\ \vert\ \bot&\neg\text{-elim }9,2\\
11&\vert\ \vert\ \vert\ \vert\ R(c_0)&\bot\text{-elim }10\\
12&\vert\ \vert\ \vert\ R(c_0)&\lor\text{-elim }5,6\text{--}7,8\text{--}11\\
13&\vert\ \vert\ R(c_0)&\exists\text{-elim }3,4\text{--}12\\
14&\vert\ (\exists x\,R(x))\to R(c_0)&\to\text{-intro }3\text{--}13\\
15&\neg R(c_1)\to((\exists x\,R(x))\to R(c_0))&\to\text{-intro }2\text{--}14
\end{array}
$$

The sibling case [subproofs](../../../../../subproof.md) end before the witness [subproof](../../../../../subproof.md) closes. At line 13, $v$ is absent from $R(c_0)$ and from all surrounding assumptions, so no [witness escape](../../../../../witness-escape.md) occurs. The final two applications of [implication introduction](../../../../../implication-introduction-rule.md) give

$$
\boxed{\forall x\,(x=c_0\lor x=c_1)\ \vdash\ \neg R(c_1)\to(\exists x\,R(x))\to R(c_0).}
$$

The [logical falsity elimination rule](../../../../../logical-falsity-elimination-rule.md) is needed to complete the contradictory second case with the same conclusion as the first case.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
