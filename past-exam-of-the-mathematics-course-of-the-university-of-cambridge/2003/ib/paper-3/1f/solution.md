<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

The [integral](../../../../../integral.md) is finite because a [continuous function](../../../../../continuous-function.md) on a [compact](../../../../../compact-space.md) [closed interval](../../../../../closed-real-interval.md) is bounded. Nonnegativity is immediate, and [absolute homogeneity of a norm](../../../../../absolute-homogeneity-of-a-norm.md) follows from $|cf(x)|=|c|\,|f(x)|$. The pointwise [triangle inequality](../../../../../triangle-inequality.md) gives

$$
\|f+g\|\leq\int_{-1}^1(|f(x)|+|g(x)|)\,dx=\|f\|+\|g\|.
$$

For positive definiteness, if $f(x_0)\ne0$, [continuity](../../../../../continuous-function.md) gives a relative interval of positive length on which $|f(x)|\geq |f(x_0)|/2$. Its [integral](../../../../../integral.md) is positive, including when $x_0$ is an endpoint. Thus $\|f\|=0$ implies $f=0$, and this is a [norm](../../../../../norm.md) on the given [vector space](../../../../../vector-space-split.md).

For the given [sequence](../../../../../sequence.md),

$$
\|f_n\|=2\int_0^1x^n\,dx=\frac2{n+1},\qquad \|f_n-f_m\|\leq\frac2{n+1}+\frac2{m+1}.
$$

The last bound tends to zero as both indices tend to infinity, proving the [Cauchy sequence](../../../../../cauchy-sequence.md) property. Moreover, **the sequence converges to the zero function in this norm**:

$$
\boxed{\|f_n-0\|=\frac2{n+1}\longrightarrow0.}
$$

There is no conflict with the nonzero endpoint values: convergence in this [norm](../../../../../norm.md) does not imply [pointwise convergence](../../../../../pointwise-convergence.md).

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
