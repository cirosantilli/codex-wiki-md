<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $f$ be the nonzero bounded [holomorphic function](../../../../../../holomorphic-function.md) in the zero-set condition. Choose $v$ with $f(v)\ne0$ and compose with a disk [Möbius transformation](../../../../../../mobius-transformation.md) carrying zero to $v$. Call the resulting function $g$ and its zeros $a_n$, counted with multiplicity. Then $g(0)\ne0$ and $|g|\leq1$.

For a radius $r$ with no zero on its circle, [Jensen's formula](../../../../../../jensen-s-formula.md) gives

$$
\sum_{|a_n|<r}\log\frac r{|a_n|}=\frac1{2\pi}\int_0^{2\pi}\log|g(re^{i\theta})|\,d\theta-\log|g(0)|\leq-\log|g(0)|.
$$

To see the formula directly, divide $g$ by its finitely many interior zero factors. The logarithm of the modulus of the resulting zero-free [holomorphic function](../../../../../../holomorphic-function.md) is harmonic near the closed disk and satisfies the [mean value property](../../../../../../mean-value-property-for-harmonic-functions.md). The circle average of $\log|re^{i\theta}-a|$ for $|a|<r$ is $\log r$, obtained by expanding $\log(1-(a/r)e^{-i\theta})$. Subtracting its value at zero gives exactly the displayed zero sum.

Let $r\uparrow1$ through zero-free circles. Increasing limits of the nonnegative summands give

$$
\sum_n-\log|a_n|\leq-\log|g(0)|<\infty.
$$

Since $1-|a_n|\leq-\log|a_n|$, the [Blaschke condition](../../../../../../blaschke-condition.md) follows for the transformed sequence. The [hyperbolic metric](../../../../../../hyperbolic-metric.md) identity and the base-point comparison proved above give

$$
\boxed{\sum_n e^{-\rho(w,z_n)}<\infty\quad\text{for every }w\in\mathbb D.}
$$

This proves the reverse implication and completes the equivalence.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
