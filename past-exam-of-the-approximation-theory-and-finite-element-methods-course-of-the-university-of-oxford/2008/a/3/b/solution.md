<h1 id="a/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $K$ has one sign, the weighted mean-value theorem applied to the continuous [derivative](../../../../../derivative.md) $u^{(n+1)}$ gives

$$
\int_0^1K(t)u^{(n+1)}(t)\,dt
=u^{(n+1)}(\eta)\int_0^1K(t)\,dt
$$

for some $\eta\in[0,1]$. One may prove this by bounding the weighted integral between the minimum and maximum [derivative](../../../../../derivative.md) values times the total weight, then using the [intermediate value theorem](../../../../../intermediate-value-theorem.md). If the total weight is zero, the fixed-sign kernel is zero almost everywhere and the conclusion is immediate.

Apply the [Peano kernel theorem](../../../../../peano-kernel-theorem.md) to $u(x)=x^{n+1}$ to get $X[x^{n+1}]=(n+1)!\int_0^1K$. Consequently

$$
\boxed{X[u]=\frac{u^{(n+1)}(\eta)}{(n+1)!}X[x^{n+1}].}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
