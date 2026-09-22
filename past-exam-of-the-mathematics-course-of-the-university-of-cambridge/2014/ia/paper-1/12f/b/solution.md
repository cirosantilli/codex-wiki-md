<h1 id="12f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a nondecreasing function, the endpoint bounds show it is bounded. On the uniform partition into $N$ intervals, its [Darboux sums](../../../../../../darboux-sum.md) satisfy

$$
U-L=\frac1N\sum_{j=1}^N\left[f\left(\frac jN\right)-f\left(\frac{j-1}N\right)\right]
=\frac{f(1)-f(0)}N\longrightarrow0.
$$

For a nonincreasing function apply the same calculation to $-f$, or use $|f(1)-f(0)|/N$. Thus **every [monotone function](../../../../../../monotonic-function.md) on $[0,1]$ is [Riemann integrable](../../../../../../riemann-integrable-function.md)**.

For the unheaded rational-weight example, each summand is nonnegative, and increasing $x$ only adds indices. Hence its sum is nondecreasing and lies between zero and one, including the separately specified value at zero. It is a [left-continuous cumulative function of an atomic measure](../../../../../../left-continuous-cumulative-function-of-an-atomic-measure.md).

If $q_j\in[0,1)$ and $q_j<x\leq1$, the index $j$ appears in the sum at $x$ but not at $q_j$. All other changes are nonnegative, so $f(x)-f(q_j)\geq2^{-j}$. This remains true for arbitrarily small positive $x-q_j$, proving discontinuity at $q_j$, including a right discontinuity at zero when that rational is encountered. Every interval of positive length contains such a rational in its interior. **The discontinuities are therefore dense**, although **the function is [Riemann integrable](../../../../../../riemann-integrable-function.md)** by the monotone-function result just proved.

More concretely, truncate after the first $N$ weights. The resulting finite sum of step functions is integrable, and the uniform tail is at most $2^{-N}$. This also proves integrability and gives, if its value is desired,

$$
\boxed{\int_0^1 f(x)\,dx=\sum_{k=1}^\infty2^{-k}(1-q_k).}
$$

The integral formula follows by integrating the finite sums and using the uniform tail bound. Here “every interval” has the usual nondegenerate-interval meaning; a singleton is not being asserted to contain a discontinuity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
