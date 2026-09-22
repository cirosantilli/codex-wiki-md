<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Differentiate the [locally uniformly convergent](../../../../../../locally-uniform-convergence.md) logarithm of the [Euler product](../../../../../../euler-product.md). Its [logarithmic derivative](../../../../../../logarithmic-derivative.md) is

$$
-\frac{\zeta'(s)}{\zeta(s)}=\sum_p\sum_{m\ge1}\frac{\log p}{p^{ms}}=\sum_{n\ge1}\frac{\Lambda(n)}{n^s},\qquad\Re s>1.
$$

The differentiated sum is [absolutely convergent](../../../../../../absolute-convergence.md), since $\Lambda(n)\le\log n$. Taking the real parts at the three heights gives

$$
-3\frac{\zeta'(\sigma)}{\zeta(\sigma)}-4\Re\frac{\zeta'(\sigma+it)}{\zeta(\sigma+it)}-\Re\frac{\zeta'(\sigma+2it)}{\zeta(\sigma+2it)}=\sum_{n\ge1}\frac{\Lambda(n)}{n^\sigma}\bigl(3+4\cos(t\log n)+\cos(2t\log n)\bigr)\ge0.
$$

Each summand is nonnegative because its bracket is $2(1+\cos(t\log n))^2$. This proves the derivative form of the [three-four-one zero-free-region argument](../../../../../../three-four-one-zero-free-region-argument.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
