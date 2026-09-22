<h1 id="4/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For convex $f$, the [subgradient inequality](../../../../../../../subgradient-inequality.md) gives

$$
f(x)-f(x_1,\ldots,z,\ldots,x_n)
\leq\partial_if(x)(x_i-z).
$$

Taking the positive supremum over $z\in[0,1]$ and summing squares shows

$$
V^+(x)\leq\sum_i(\partial_if(x))^2\leq1.
$$

The [modified logarithmic Sobolev inequality](../../../../../../../modified-logarithmic-sobolev-inequality.md) from part a with $v=1$ therefore gives

$$
\boxed{\mathbb P(Z-\mathbb EZ\geq t)\leq e^{-t^2/2}.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 208](../../../../paper-208-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
