<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $k=\Delta t>0$ and retain the same [matrix](../../../../../../matrix.md) $L$. The [Crank-Nicolson method](../../../../../../crank-nicolson-method.md) is

$$
U^{n+1}-U^n=\frac{k}{2}L(U^{n+1}+U^n).
$$

Take the real mesh-weighted inner product with $U^{n+1}+U^n$. The cross terms cancel, and the identity from part (b) gives

$$
\|U^{n+1}\|_d^2-\|U^n\|_d^2
=\frac{k}{2}\operatorname{Re}\langle L(U^{n+1}+U^n),U^{n+1}+U^n\rangle_d
\leq0.
$$

The implicit system is uniquely solvable: if $(I-kL/2)V=0$, then

$$
\|V\|_d^2=\frac{k}{2}\operatorname{Re}\langle LV,V\rangle_d\leq0,
$$

so $V=0$. Therefore its [dissipative Cayley-transform contraction](../../../../../../dissipative-cayley-transform-contraction.md) satisfies

$$
\boxed{\left\|\left(I-\frac{k}{2}L\right)^{-1}
\left(I+\frac{k}{2}L\right)\right\|_2\leq1.}
$$

Iterating proves **unconditional stability for every $\mu=k/d^2>0$**; the perturbation bound is one and does not depend on the mesh or time-step ratio.

The printed hint's exponential estimate is valid with the logarithmic norm, but its proposed bound by $r(k\alpha[L])$ is not a general inheritance principle. For the trapezoidal [stability function](../../../../../../stability-function.md) $r(z)=(1+z/2)/(1-z/2)$, that real number can even be negative when $k\alpha[L]<-2$, whereas a norm is nonnegative. The direct energy proof above establishes the required result without that assertion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
