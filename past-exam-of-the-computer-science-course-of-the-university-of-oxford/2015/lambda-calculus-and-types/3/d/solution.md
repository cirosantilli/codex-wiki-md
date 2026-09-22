<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Successive [bracket abstractions](../../../../../bracket-abstraction.md) are processed from the inside out: $[x][y]((\mathbf Kx)y)$. Retain $I\equiv(\mathbf S\mathbf K)\mathbf K$ only as a temporary abbreviation for the [I combinator](../../../../../i-combinator.md). Since $y$ is absent from $\mathbf Kx$, the first [bracket abstraction](../../../../../bracket-abstraction.md) is

$$
[y]((\mathbf Kx)y)
\equiv\mathbf S\bigl(\mathbf K(\mathbf Kx)\bigr)I.
$$

For the outer [bracket abstraction](../../../../../bracket-abstraction.md), $x$ is absent from $I$ and the [S combinator](../../../../../s-combinator.md), while it occurs in $\mathbf K(\mathbf Kx)$. Hence

$$
\begin{aligned}
[x]\bigl(\mathbf S(\mathbf K(\mathbf Kx))I\bigr)
&\equiv\mathbf S\bigl([x](\mathbf S(\mathbf K(\mathbf Kx)))\bigr)(\mathbf KI),\\
[x](\mathbf S(\mathbf K(\mathbf Kx)))
&\equiv\mathbf S(\mathbf K\mathbf S)\bigl([x](\mathbf K(\mathbf Kx))\bigr),\\
[x](\mathbf K(\mathbf Kx))
&\equiv\mathbf S(\mathbf K\mathbf K)\bigl([x](\mathbf Kx)\bigr),\\
[x](\mathbf Kx)
&\equiv\mathbf S(\mathbf K\mathbf K)I.
\end{aligned}
$$

Substituting upward and then expanding $I$ gives the following fully bracketed string, consisting solely of the [S combinator](../../../../../s-combinator.md), the [K combinator](../../../../../k-combinator.md) and parentheses:

$$
\boxed{
\left(
\left(\mathbf S
\left(
\left(\mathbf S(\mathbf K\mathbf S)\right)
\left(
\left(\mathbf S(\mathbf K\mathbf K)\right)
\left(\left(\mathbf S(\mathbf K\mathbf K)\right)\left((\mathbf S\mathbf K)\mathbf K\right)\right)
\right)
\right)
\right)
\left(\mathbf K\left((\mathbf S\mathbf K)\mathbf K\right)\right)
\right).
}
$$

For readability, the same result with the usual left association convention and the temporary abbreviation is

$$
\mathbf S\bigl(\mathbf S(\mathbf K\mathbf S)
(\mathbf S(\mathbf K\mathbf K)(\mathbf S(\mathbf K\mathbf K)I))\bigr)(\mathbf KI).
$$

The syntactic result comes from the specified [bracket abstraction](../../../../../bracket-abstraction.md) algorithm. Replacing it by the shorter [K combinator](../../../../../k-combinator.md), despite agreement after two arguments, would not answer the requested computation. As a check using the result of part (b), applying the computed [combinatory logic term](../../../../../combinatory-logic-term.md) to $u,v$ gives $\mathbf Kuv=u$.

## ↑ Ancestors (11)

1. [D](../d.md)
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
