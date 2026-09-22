<h1 id="40d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Householder-John theorem](../../../../../../householder-john-theorem.md) states the following. Let

$$
A=M-N
$$

be a splitting in which $A$ is Hermitian positive definite. If

$$
B=M^*+N
$$

is also Hermitian positive definite, then $M$ is nonsingular and every eigenvalue of $H=M^{-1}N$ has modulus less than one. Hence the associated stationary iteration converges.

First, $M$ must be nonsingular. If $Mx=0$ for some nonzero $x$, then $Nx=-Ax$, and therefore

$$
x^*Bx=x^*(M^*+N)x=-x^*Ax<0,
$$

contradicting the positive definiteness of $B$.

Now let $Hx=\lambda x$ with $x\ne0$. Then $Nx=\lambda Mx$, so

$$
Ax=(1-\lambda)Mx.
$$

Put $a=x^*Ax>0$ and $m=x^*Mx$. Since $\lambda\ne1$,

$$
m=\frac{a}{1-\lambda}.
$$

Consequently,

$$
0<x^*Bx
=\overline m+\lambda m
=a\left(\frac1{1-\overline\lambda}
+\frac{\lambda}{1-\lambda}\right)
=a\frac{1-|\lambda|^2}{|1-\lambda|^2}.
$$

It follows that $|\lambda|<1$. Thus $\rho(H)<1$, proving the theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40D](../../40d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
