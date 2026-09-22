<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $f(x)=\operatorname{TS}\{x_1,\ldots,x_n\}$. Besides [Talagrand's convex distance inequality](../../../../../../talagrand-s-convex-distance-inequality.md), we use the precise [squared edge bound for tours in the unit square](../../../../../../squared-edge-bound-for-tours-in-the-unit-square.md) stated above and the [triangle inequality](../../../../../../triangle-inequality.md), which permits shortcutting a [closed walk](../../../../../../closed-walk.md) without increasing its length. We first prove the geometric comparison that connects these results.

For each fixed $x$, choose a cyclic tour $C$ with edge lengths $\ell_i$ satisfying $\sum_i\ell_i^2\leq4$. At vertex $x_i$, let $a_i(x)$ be the sum of the lengths of its two incident edges in $C$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\sum_i a_i(x)^2\leq4\sum_i\ell_i^2\leq16.
$$

We claim the [weighted mismatch bound for Euclidean tours](../../../../../../weighted-mismatch-bound-for-euclidean-tours.md):

$$
f(x)-f(y)\leq\sum_{i:x_i\ne y_i}a_i(x)\qquad\text{for every }y.
$$

To prove it, keep the vertices whose coordinates agree. In the cyclic ordering $C$, the deleted vertices split into consecutive runs between kept vertices. For one run, let $a,b$ denote its two boundary edge lengths and $S$ the sum of its internal edge lengths. Starting at the left kept endpoint, visit the run and return along the same path, at cost $2(a+S)$; starting at the right endpoint costs $2(b+S)$. Choose the cheaper detour. Its cost is at most

$$
2S+2\min(a,b)\leq2S+a+b,
$$

which is exactly the sum of $a_i(x)$ over that run. Attach these detours to a shortest tour through $y$, which already visits every kept point. The resulting [closed walk](../../../../../../closed-walk.md) visits all points of $x$; shortcut it using the [triangle inequality](../../../../../../triangle-inequality.md). Summing the detour costs proves the claimed [weighted mismatch bound for Euclidean tours](../../../../../../weighted-mismatch-bound-for-euclidean-tours.md). If there is just one kept vertex, the same argument uses that vertex as both endpoints of the unique run. If there are no kept vertices, $f(x)\leq\sum_i\ell_i\leq\sum_i a_i(x)$ proves the comparison directly. Repeated point locations cause no difficulty, since their connecting edges may have length zero.

Let $M$ be any [median](../../../../../../median.md) of $f(X)$ and set $A=\{y:f(y)\leq M\}$. For $f(x)\geq M+t$, the [weighted mismatch bound for Euclidean tours](../../../../../../weighted-mismatch-bound-for-euclidean-tours.md) implies

$$
\inf_{y\in A}\sum_{i:x_i\ne y_i}\frac{a_i(x)}4\geq\frac t4.
$$

The weights have squared sum at most one, so $d_T(x,A)\geq t/4$. Since $\mathbb P(A)\geq1/2$, [Talagrand's convex distance inequality](../../../../../../talagrand-s-convex-distance-inequality.md) yields

$$
\mathbb P(f(X)\geq M+t)\leq2e^{-t^2/64}.
$$

For the lower tail, put $B=\{x:f(x)\leq M-t\}$. If $\mathbb P(B)=0$ there is nothing to prove. For every $y$ with $f(y)\geq M$, apply the same [weighted mismatch bound for Euclidean tours](../../../../../../weighted-mismatch-bound-for-euclidean-tours.md) with its weights $a_i(y)$ and all $x\in B$. It gives $d_T(y,B)\geq t/4$. The set of such $y$ has probability at least $1/2$, so [Talagrand's convex distance inequality](../../../../../../talagrand-s-convex-distance-inequality.md) instead gives

$$
\mathbb P(B)\cdot\frac12\leq e^{-t^2/64}.
$$

Combining both tails,

$$
\boxed{\mathbb P(|Y_n-M_{Y_n}|\geq t)\leq4e^{-t^2/64}\qquad(t>0).}
$$

**The bound has a constant fluctuation scale, independent of $n$.** Only independence of the point coordinates and their support in the square are needed here; their [uniform distribution](../../../../../../continuous-uniform-distribution.md) was needed for the earlier lower bound on the [expected value](../../../../../../expected-value.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 112](../../../paper-112-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
