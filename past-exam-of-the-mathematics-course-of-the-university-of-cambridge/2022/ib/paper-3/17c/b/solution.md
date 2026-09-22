<h1 id="17c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md) says that a consistent linear multistep method is convergent exactly when it is zero-stable. Here

$$
\rho(z)=z^3+(2a-3)z^2-(2a-3)z-1
=(z-1)\bigl(z^2+2(a-1)z+1\bigr).
$$

The consistency conditions hold for every $a$. The two quadratic roots have product one. They are distinct and on the unit circle exactly when $0<a<2$; at $a=2$ the root $-1$ is repeated, while outside this interval one root has modulus greater than one. The [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) therefore gives

$$
\boxed{\text{convergence exactly for }0<a<2}.
$$

The polynomial exactness conditions hold through degree two, while the degree-three residual is $6-a$. Every convergent member thus has

$$
\boxed{\text{order }2}.
$$

(The exceptional value $a=6$ has formal order four but is not zero-stable.)

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17C](../../17c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
