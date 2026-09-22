<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Again write $[x]A$ for [bracket abstraction](../../../../../bracket-abstraction.md). In [combinatory logic](../../../../../combinatory-logic.md), all variable occurrences are [free variables](../../../../../free-variable.md). Under $x\neq y$ and $x\notin FV(B)$, [substitution](../../../../../substitution-algebra.md) for $y$ preserves the presence or absence of $x$:

$$
x\in FV(C[B/y])\quad\Longleftrightarrow\quad x\in FV(C).
$$

An existing $x$ is not replaced because $x\neq y$; replacing $y$ cannot introduce an $x$ because $B$ contains none. This ensures that the same clause of [bracket abstraction](../../../../../bracket-abstraction.md) applies before and after [substitution](../../../../../substitution-algebra.md).

Use [structural induction](../../../../../structural-induction.md) on $A$, respecting those clauses. If $A\equiv x$, then

$$
([x]x)[B/y]\equiv\mathbf{SKK}
\equiv[x]x
\equiv[x](x[B/y]),
$$

because [substitution](../../../../../substitution-algebra.md) leaves the [S combinator](../../../../../s-combinator.md), the [K combinator](../../../../../k-combinator.md) and $x$ unchanged.

If $x$ is absent from $A$, it is also absent from $A[B/y]$. Therefore

$$
([x]A)[B/y]
\equiv(\mathbf KA)[B/y]
\equiv\mathbf K(A[B/y])
\equiv[x](A[B/y]).
$$

This includes $A\equiv y$: even when $B$ is a large application, the absence of $x$ means [bracket abstraction](../../../../../bracket-abstraction.md) still produces $\mathbf KB$.

Finally, let $A\equiv CD$ with $x$ occurring in $C$ or $D$. By the occurrence observation, $x$ also occurs in $C[B/y]$ or $D[B/y]$, so the application clause applies on both sides. Apply the induction hypotheses:

$$
\begin{aligned}
([x](CD))[B/y]
&\equiv\bigl(\mathbf S([x]C)([x]D)\bigr)[B/y]\\
&\equiv\mathbf S\bigl(([x]C)[B/y]\bigr)\bigl(([x]D)[B/y]\bigr)\\
&\equiv\mathbf S\bigl([x](C[B/y])\bigr)\bigl([x](D[B/y])\bigr)\\
&\equiv[x]\bigl(C[B/y]D[B/y]\bigr)\\
&\equiv[x]\bigl((CD)[B/y]\bigr).
\end{aligned}
$$

Every step uses the definitions of [substitution](../../../../../substitution-algebra.md) and [bracket abstraction](../../../../../bracket-abstraction.md), without applying the equality axioms for the [S combinator](../../../../../s-combinator.md) or the [K combinator](../../../../../k-combinator.md). Thus the result is the stronger syntactic identity

$$
\boxed{([x]A)[B/y]\equiv[x](A[B/y]).}
$$

The side condition on $B$ is essential for this identity. For example, substituting $x$ for $y$ in $[x]y\equiv\mathbf Ky$ gives $\mathbf Kx$, whereas $[x](y[x/y])\equiv[x]x\equiv\mathbf{SKK}$, a different string.

## ↑ Ancestors (11)

1. [C](../c.md)
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
