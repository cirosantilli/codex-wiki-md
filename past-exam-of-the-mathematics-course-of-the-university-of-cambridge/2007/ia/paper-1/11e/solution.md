<h1 id="11e/solution">Solution</h1>

↑ **Parent:** [11E](../11e.md)

To prove boundedness on $[a,b]$, suppose instead that $f$ is unbounded and choose $x_n\in[a,b]$ with $|f(x_n)|>n$. The [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md) gives a subsequence converging to $x_*\in[a,b]$. [Continuity](../../../../../continuous-function.md) then gives $f(x_{n_j})\to f(x_*)$, contradicting $|f(x_{n_j})|>n_j$. Hence $f$ is bounded.

Let $M=\sup_{x\in[a,b]}f(x)$ and $m=\inf_{x\in[a,b]}f(x)$. Choose $d_n$ with $M-1/n<f(d_n)\leq M$. Another application of [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md) yields a subsequence tending to $d\in[a,b]$, and [continuity](../../../../../continuous-function.md) gives $f(d)=M$. Applying the same argument to $-f$ gives $c\in[a,b]$ with $f(c)=m$. Thus

$$
\boxed{f(c)\leq f(x)\leq f(d)\quad\text{for all }x\in[a,b].}
$$

This proves the [extreme value theorem](../../../../../extreme-value-theorem.md) here, including both attainment assertions.

For $g$, its two limits supply $R>0$ such that $|g(x)|<1$ whenever $|x|>R$. On $[-R,R]$, [continuity](../../../../../continuous-function.md) and the result just proved give a finite bound $K$. Consequently **$|g(x)|\leq\max\{K,1\}$ on the whole real line**.

For the final value assertion, if $c=g(a)$, take $x=a$. Otherwise $0<c<g(a)$. The positive-infinity [limit](../../../../../limit-of-a-function.md) gives a point $b>a$ with $|g(b)|<c$, so $g(b)<c<g(a)$. The [intermediate value theorem](../../../../../intermediate-value-theorem.md) on $[a,b]$ now gives $x\in(a,b)$ with

$$
\boxed{g(x)=c.}
$$

Positivity of $c$ is essential to this tail argument; a function can tend to zero without ever attaining zero.

## ↑ Ancestors (10)

1. [11E](../11e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
