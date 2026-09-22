<h1 id="14e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

At $c=0$ the left-hand root is $-2$, and the derivative of the polynomial with respect to $z$ is $3(-2)^2=12\ne0$. The [holomorphic implicit function theorem](../../../../../../holomorphic-implicit-function-theorem.md) states that if $P(z,c)$ is holomorphic near $(z_0,c_0)$, $P(z_0,c_0)=0$ and $P_z(z_0,c_0)\ne0$, there is a unique holomorphic function $z=\gamma(c)$ near $c_0$, with $\gamma(c_0)=z_0$ and $P(\gamma(c),c)=0$. It therefore supplies an analytic root branch $\gamma(c)$ near zero. Differentiate its equation:

$$
(3\gamma(c)^2+ic)\gamma'(c)+i\gamma(c)=0.
$$

It follows that $\gamma'(0)=i/6$ and

$$
\boxed{\gamma(c)=-2+\frac{i}{6}c+O(c^2).}
$$

For sufficiently small positive $c$ its imaginary part is $c/6+O(c^2)>0$. By the unique-root localization from the preceding part, this is the root in the left half-plane. Thus **that root lies above the real axis for all sufficiently small positive $c$**.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [14E](../../14e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
