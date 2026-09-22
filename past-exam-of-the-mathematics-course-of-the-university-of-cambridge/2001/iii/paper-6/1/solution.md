<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Start with the [approximate surjectivity with geometric correction](../../../../../approximate-surjectivity-with-geometric-correction.md) argument. For a fixed $y$, put $r_0=y$. Choose $x_j$ successively so that

$$
\|x_j\|\le R\|r_{j-1}\|,\qquad r_j=r_{j-1}-Tx_j,\qquad \|r_j\|\le k\|r_{j-1}\|.
$$

Induction gives $\|r_j\|\le k^j\|y\|$ and $\|x_j\|\le Rk^{j-1}\|y\|$. The series $\sum_jx_j$ is absolutely convergent in the [Banach space](../../../../../banach-space-split.md) $V$, because the sum of its norms is bounded by the convergent [geometric series](../../../../../geometric-series.md) $R\|y\|/(1-k)$. Write its sum as $x$. The [bounded linear operator](../../../../../continuous-linear-operator.md) $T$ commutes with this limit, while $T\sum_{j=1}^m x_j=y-r_m\to y$. Consequently

$$
\boxed{Tx=y,\qquad \|x\|\le\frac{R}{1-k}\|y\|.}
$$

The choices need not depend linearly on $y$; no bounded linear right inverse is being asserted.

For the bounded extension, use the restriction [bounded linear operator](../../../../../continuous-linear-operator.md) $S:C_b(X;\mathbb R)\to C_b(Y;\mathbb R)$ on the [Banach spaces](../../../../../banach-space-split.md) of [bounded continuous functions](../../../../../bounded-continuous-functions.md), each with its [supremum norm](../../../../../supremum-norm.md). We will construct an approximation to any $g$ with $\|g\|_\infty=M>0$. The two sets

$$
A=\{y\in Y:g(y)\le -M/3\},\qquad B=\{y\in Y:g(y)\ge M/3\}
$$

are disjoint [closed sets](../../../../../closed-set.md) in $X$, since $Y$ is closed. If both are nonempty, the [distance to a set](../../../../../distance-to-a-set.md) construction defines a [continuous function](../../../../../continuous-function.md)

$$
u(x)=\frac M3\frac{d(x,A)-d(x,B)}{d(x,A)+d(x,B)}.
$$

The denominator is positive at every point: zero distance to a closed set means membership in that set. Thus $\|u\|_\infty\le M/3$, with $u=-M/3$ on $A$ and $u=M/3$ on $B$. On $A$ and $B$, and also on the intervening range $|g|<M/3$, this implies

$$
\|Su-g\|_\infty\le 2M/3.
$$

If only $A$ is empty take $u=M/3$, if only $B$ is empty take $u=-M/3$, and if both are empty take $u=0$; the same bounds hold. For $M=0$ take $u=0$. This proves the approximation hypothesis with $R=1/3$ and $k=2/3$. Applying the argument above to $S$ yields an element $h$ of the [bounded continuous functions](../../../../../bounded-continuous-functions.md) with $h|_Y=g$ and $\|h\|_\infty\le\|g\|_\infty$. Restriction gives the reverse inequality, so **the extension preserves the exact supremum norm**:

$$
\boxed{\|h\|_\infty=\|g\|_\infty.}
$$

This proves the bounded metric-space case of the [Tietze extension theorem](../../../../../tietze-extension-theorem.md) rather than presupposing it.

For an arbitrary real [continuous function](../../../../../continuous-function.md) $f$ on $Y$, let $g=\tanh f$. Its values lie strictly between $-1$ and $1$, although its supremum norm can be $1$. The bounded result supplies an extension $h$ with $|h|\le1$. Let $D=\{x:|h(x)|=1\}$, a [closed set](../../../../../closed-set.md) disjoint from $Y$. If $D$ is nonempty and $Y$ is nonempty, put

$$
\eta(x)=\frac{d(x,D)}{d(x,D)+d(x,Y)},\qquad q(x)=\eta(x)h(x).
$$

Both factors are [continuous functions](../../../../../continuous-function.md); $\eta=1$ on $Y$ and $\eta=0$ on $D$. Off $D$ we have $|h|<1$, and on $D$ we have $q=0$, so $|q(x)|<1$ everywhere. Therefore **a real continuous extension is**

$$
\boxed{F(x)=\operatorname{arctanh}q(x).}
$$

On $Y$ it equals $f$. If $D$ is empty use $q=h$; if $Y$ is empty simply take $F=0$. This handles unbounded $f$ without requiring a uniform margin between $|g|$ and $1$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
