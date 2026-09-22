<h1 id="7/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The stated weighted [inequality](../../../../../../../inequality-mathematics.md) is the [Jensen inequality](../../../../../../../jensen-s-inequality.md) for a [concave function](../../../../../../../concave-function.md). Assume $a<b$; if $a=b$, both sides of the required [inequality](../../../../../../../inequality-mathematics.md) are zero. Write $x=\lambda a+(1-\lambda)b$ with $\lambda=(b-x)/(b-a)$. Applying the weighted [inequality](../../../../../../../inequality-mathematics.md) at the two endpoints gives

$$
f(x)\geq\ell(x)=\frac{b-x}{b-a}f(a)+\frac{x-a}{b-a}f(b).
$$

Thus the [affine function](../../../../../../../affine-function.md) $\ell$ joining the endpoint values lies below $f$. By [monotonicity of the Riemann integral](../../../../../../../monotonicity-of-the-riemann-integral.md),

$$
\int_a^b f(x)\,dx\geq\int_a^b\ell(x)\,dx
=\boxed{\frac{b-a}{2}\bigl(f(a)+f(b)\bigr).}
$$

This is the lower bound in the [Hermite-Hadamard inequality](../../../../../../../hermite-hadamard-inequality.md) for a [concave function](../../../../../../../concave-function.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
