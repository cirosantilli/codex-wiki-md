<h1 id="21f/solution">Solution</h1>

↑ **Parent:** [21F](../21f.md)

A based loop is a continuous map $\alpha:[0,1]\to X$ with $\alpha(0)=\alpha(1)=x_0$. Two loops are equivalent when they are joined by a homotopy that keeps both endpoints at $x_0$. The [fundamental group](../../../../../fundamental-group.md) $\pi_1(X,x_0)$ is the set of these based-homotopy classes.

For loops $\alpha$ and $\beta$, define concatenation by

$$
(\alpha*\beta)(t)=
\begin{cases}
\alpha(2t),&0\leq t\leq\tfrac12,\\
\beta(2t-1),&\tfrac12\leq t\leq1.
\end{cases}
$$

If $H$ and $K$ are based homotopies from $\alpha$ to $\alpha'$ and from $\beta$ to $\beta'$, concatenating $H(s,-)$ and $K(s,-)$ gives a based homotopy from $\alpha*\beta$ to $\alpha'*\beta'$. Thus multiplication $[\alpha][\beta]=[\alpha*\beta]$ is well-defined.

Concatenating three paths with different breakpoints changes only the speed of traversal. Linear interpolation between the two increasing piecewise-linear parametrizations gives a based homotopy, proving associativity on classes. The constant loop $c(t)=x_0$ is an identity, since deleting its stationary half is another endpoint-fixing reparametrization. The inverse of $[\alpha]$ is represented by $\bar\alpha(t)=\alpha(1-t)$. Indeed, $\alpha*\bar\alpha$ contracts through

$$
H(s,t)=
\begin{cases}
\alpha(2t(1-s)),&0\leq t\leq\tfrac12,\\
\alpha(2(1-t)(1-s)),&\tfrac12\leq t\leq1,
\end{cases}
$$

and the analogous contraction handles $\bar\alpha*\alpha$. Hence the operation satisfies all group axioms.

## ↑ Ancestors (10)

1. [21F](../21f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
