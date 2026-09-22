<h1 id="18c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For this [Adams–Moulton method](../../../../../../adams-moulton-method.md), the [characteristic polynomials of a linear multistep method](../../../../../../characteristic-polynomials-of-a-linear-multistep-method.md) are

$$
\rho(w)=w^2-w,
\qquad
\sigma(w)=\frac{5w^2+8w-1}{12}.
$$

Expansion at zero gives

$$
\rho(e^z)-z\sigma(e^z)=-\frac1{24}z^4+O(z^5).
$$

Part (a) therefore shows that the method has order exactly three.

It is consistent because its order is at least one. The roots of $\rho(w)=w(w-1)$ are $0$ and $1$; both lie in the closed unit disk, and the only unit-modulus root is simple. Thus the method is [zero-stable](../../../../../../zero-stability.md). By the [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md), consistency and zero stability imply convergence. Hence the method is

$$
\boxed{\text{third-order and convergent}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18C](../../18c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
