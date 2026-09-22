<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The argument order in $p$ is a [cyclic permutation](../../../../../cyclic-permutation.md). Undo it by rotating in the other direction. For $n\geq1$, choose the [lambda term](../../../../../lambda-term.md)

$$
\boxed{q\equiv\lambda z y_1\cdots y_n.\,z\,y_n\,y_1\cdots y_{n-1}.}
$$

Use fresh bound variables throughout. Substituting $qz$ for the first argument of $p$ and then performing [beta reduction](../../../../../beta-reduction.md) gives

$$
\begin{aligned}
(p\bullet q)z
&\longrightarrow_\beta^*p(qz)\\
&\longrightarrow_\beta^*\lambda x_1\cdots x_n.\,(qz)x_2\cdots x_nx_1\\
&\longrightarrow_\beta^*\lambda x_1\cdots x_n.\,zx_1\cdots x_n.
\end{aligned}
$$

Indeed, the arguments received by $qz$ are $y_1=x_2,\ldots,y_{n-1}=x_n,y_n=x_1$, so its last argument moves back to the front. Apply [eta conversion](../../../../../eta-conversion.md) successively, starting with the innermost [lambda abstraction](../../../../../lambda-abstraction.md). At each step the bound variable being removed is absent from the preceding expression. Thus the last expression is related to $z$ by [beta-eta equivalence](../../../../../beta-eta-equivalence.md), and consequently

$$
\boxed{p\bullet q=_{\beta\eta}\lambda z.z=I.}
$$

For the induction needed in the next part, also compute the reverse [composition of lambda terms](../../../../../composition-of-lambda-terms.md):

$$
\begin{aligned}
(q\bullet p)z
&\longrightarrow_\beta^*\lambda y_1\cdots y_n.\,(pz)y_ny_1\cdots y_{n-1}\\
&\longrightarrow_\beta^*\lambda y_1\cdots y_n.\,zy_1\cdots y_n
=_\eta z.
\end{aligned}
$$

So this $q$ is a two-sided inverse. The empty argument list at $n=0$ means $p=\lambda z.z$; choose $q=I$. For $n=1$, both displayed rotations give $\lambda zy_1.zy_1$, which is also related to $I$ by [eta conversion](../../../../../eta-conversion.md). These boundary cases require no exceptional inverse construction.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Lambda calculus and types](../../../lambda-calculus-and-types-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
