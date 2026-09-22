<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At a fixed $t$, write $A=f(t)$ and $B=f'(t)$. Differentiating the [matrix exponential](../../../../../../matrix-exponential.md) in the direction $B$ gives

$$
\boxed{\frac{d}{dt}e^{f(t)}=\int_0^1e^{(1-u)f(t)}f'(t)e^{uf(t)}\,du.}
$$

The order of factors matters because [matrix multiplication](../../../../../../matrix-multiplication.md) need not be commutative.

To prove the [derivative of the matrix exponential](../../../../../../derivative-of-the-matrix-exponential.md) formula, expand its [power series](../../../../../../power-series.md). The coefficient linear in $h$ in $(A+hB)^k$ is $\sum_{j=0}^{k-1}A^jBA^{k-1-j}$. On bounded sets of [matrices](../../../../../../matrix.md), the exponential series and its directional derivative series converge uniformly: the latter is dominated in [operator norm](../../../../../../operator-norm.md) by $\|B\|\sum_{k\geq1}k\|A\|^{k-1}/k!$. Terms with two or more $hB$ factors have sum $O(h^2)$ locally. Hence the derivative is

$$
\sum_{k\geq1}\frac1{k!}\sum_{j=0}^{k-1}A^jBA^{k-1-j}.
$$

On the other hand, the integral in the box expands absolutely as

$$
\sum_{a,b\geq0}\frac{A^aBA^b}{a!b!}\int_0^1(1-u)^au^b\,du
=\sum_{a,b\geq0}\frac{A^aBA^b}{(a+b+1)!}.
$$

The integral identity follows by repeated [integration by parts](../../../../../../integration-by-parts.md). Grouping by $a+b=k-1$ gives the same derivative. Finally differentiability means $f(t+h)=A+hB+o(h)$; the locally bounded derivative of the exponential sends the $o(h)$ error to $o(h)$, proving the chain rule even when $f'$ is not continuous. If $[f,f']=0$, the formula simplifies to $e^ff'$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
