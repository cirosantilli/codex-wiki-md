<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $[x]A$ for the paper's [bracket abstraction](../../../../../bracket-abstraction.md) and $I\equiv\mathbf{SKK}$ for the [I combinator](../../../../../i-combinator.md). Prove the result by [structural induction](../../../../../structural-induction.md) following the three clauses of [bracket abstraction](../../../../../bracket-abstraction.md).

For $A\equiv x$, the rules for the [S combinator](../../../../../s-combinator.md) and the [K combinator](../../../../../k-combinator.md) give

$$
([x]x)B\equiv\mathbf{SKK}B
=\mathbf KB(\mathbf KB)=B
\equiv x[B/x].
$$

If $x$ does not occur in $A$, then [substitution](../../../../../substitution-algebra.md) for $x$ leaves $A$ unchanged and

$$
([x]A)B\equiv\mathbf KAB=A\equiv A[B/x].
$$

These two cases cover all variables and constants as well as applications not containing $x$.

In the remaining case, $A\equiv CD$ and $x$ occurs in at least one of $C,D$. The [bracket abstraction](../../../../../bracket-abstraction.md) clause, the rule for the [S combinator](../../../../../s-combinator.md), the induction hypotheses and compatibility of equality with application give

$$
\begin{aligned}
([x](CD))B
&\equiv\mathbf S([x]C)([x]D)B\\
&=(([x]C)B)(([x]D)B)\\
&=C[B/x]D[B/x]\\
&\equiv(CD)[B/x].
\end{aligned}
$$

The last line is the defining application clause of [substitution](../../../../../substitution-algebra.md). Therefore

$$
\boxed{([x]A)B=A[B/x]\quad\text{for all }A,B.}
$$

The conclusion is equality in [combinatory logic](../../../../../combinatory-logic.md); it need not be literal identity of strings. There are no binders in a [combinatory logic term](../../../../../combinatory-logic-term.md), so this [substitution](../../../../../substitution-algebra.md) introduces no [variable capture](../../../../../variable-capture.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Lambda calculus and types](../../../lambda-calculus-and-types-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
