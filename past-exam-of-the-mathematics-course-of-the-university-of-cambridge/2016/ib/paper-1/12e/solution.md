<h1 id="12e/solution">Solution</h1>

↑ **Parent:** [12E](../12e.md)

For $q\in\mathbb Q\setminus\{0\}$ write $q=p^k u/v$, where $k\in\mathbb Z$ and neither integer $u$ nor integer $v$ is divisible by $p$. Define the [P-adic valuation](../../../../../p-adic-valuation.md) $v_p(q)=k$ and the [p-adic absolute value](../../../../../p-adic-absolute-value.md) $|q|_p=p^{-k}$, with $|0|_p=0$. **The p-adic metric** is

$$
\boxed{d_p(a,b)=|a-b|_p.}
$$

Factoring out the smaller power of $p$ from two rational numbers shows $v_p(q+r)\geq\min\{v_p(q),v_p(r)\}$, with the usual convention $v_p(0)=+\infty$. Consequently the [ultrametric inequality](../../../../../ultrametric-inequality.md) gives

$$
d_p(a,b)=|(a-c)+(c-b)|_p\leq\max\{d_p(a,c),d_p(c,b)\}.
$$

Together with symmetry, positivity and separation of points, this verifies that $d_p$ is a [metric](../../../../../metric.md).

For the given geometric partial sums, use the finite [geometric series](../../../../../geometric-series.md) identity. Since $p$ does not divide $p-1$,

$$
a_n=\frac{p^n-1}{p-1},\qquad \left|a_n+\frac1{p-1}\right|_p=\left|\frac{p^n}{p-1}\right|_p=p^{-n}\longrightarrow0.
$$

Thus **the limit is the rational number** $\boxed{1/(1-p)}$, even though the partial sums diverge in the ordinary real [metric](../../../../../metric.md).

If $|a|_p>|b|_p$, the [ultrametric inequality](../../../../../ultrametric-inequality.md) gives $|a+b|_p\leq|a|_p$. Applying it to $a=(a+b)-b$ gives $|a|_p\leq\max\{|a+b|_p,|b|_p\}$. Since $|b|_p<|a|_p$, this forces $|a+b|_p=|a|_p$. Interchanging $a,b$ handles the other unequal case, proving

$$
\boxed{|a+b|_p=\max\{|a|_p,|b|_p\}\quad\text{when }|a|_p\ne|b|_p.}
$$

Finally, let $b$ be outside the [open ball](../../../../../open-ball.md) $B(a,\delta)$, so $d_p(a,b)\geq\delta$. If $d_p(b,c)<\delta$, the preceding unequal-norm identity gives $d_p(a,c)=d_p(a,b)\geq\delta$. Therefore $B(b,\delta)$ also lies outside $B(a,\delta)$. Its complement is [open](../../../../../open-set.md), so **every p-adic open ball is also closed**, that is, a [clopen set](../../../../../clopen-set.md).

## ↑ Ancestors (10)

1. [12E](../12e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
