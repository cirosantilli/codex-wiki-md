<h1 id="19h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

We prove the [conjugate product of a quadratic ideal](../../../../../../conjugate-product-of-a-quadratic-ideal.md) identity $\mathfrak a\overline{\mathfrak a}=(N(\mathfrak a))$, which applies to the given two-generator [ideal](../../../../../../ideal.md) without assuming its displayed generators form an [integral basis](../../../../../../integral-basis.md).

The quadratic [ring of integers of a number field](../../../../../../ring-of-integers.md) has a basis $1,\omega$ over $\mathbb Z$: the vector 1 is primitive, since a rational [algebraic integer](../../../../../../algebraic-integer.md) must be an integer, and extends to an [integral basis](../../../../../../integral-basis.md). Write $\omega^2-T\omega+U=0$, with $T,U\in\mathbb Z$. Let $B$ be the least positive integer in $\mathfrak a$ and let $s>0$ generate the [set](../../../../../../set-split.md) of coefficients of $\omega$ in elements of $\mathfrak a$. Its lattice basis can be chosen as $B,r+s\omega$, with $r\in\mathbb Z$. Since $B\omega\in\mathfrak a$, comparison of coefficients shows $s\mid B$ and $s\mid r$. Write $B=sd$, $r=se$ and $\theta=e+\omega$. Then

$$
\mathfrak a=s\langle d,\theta\rangle_{\mathbb Z},
\qquad \theta+\bar\theta=T'=T+2e,\quad
\theta\bar\theta=U'=e^2+eT+U.
$$

The scaled [ideal](../../../../../../ideal.md) $\mathfrak j=s^{-1}\mathfrak a$ remains an $\mathcal O_L$-ideal. From $\theta^2-T'\theta+U'=0$ we get $U'\in\mathfrak j\cap\mathbb Z=d\mathbb Z$, so $d\mid U'$. The product $\mathfrak j\bar{\mathfrak j}$ is generated as an [ideal](../../../../../../ideal.md) by $d^2,d\theta,d\bar\theta,U'$ and is contained in $(d)$.

Moreover $\gcd(d,T',U'/d)=1$. If a prime $\ell$ divided all three, then $\ell\mid T'$ and $\ell^2\mid U'$, so $\theta/\ell$ would satisfy the monic integer [polynomial](../../../../../../polynomial-split.md) $z^2-(T'/\ell)z+U'/\ell^2$. It would lie in $\mathcal O_L$, impossible because its $\omega$ coefficient in the [integral basis](../../../../../../integral-basis.md) is $1/\ell$. [Bezout identity](../../../../../../bezout-identity.md) now expresses one as an integer combination of $d,T',U'/d$. Multiplying by $d$, the terms are $d^2$, $dT'=d\theta+d\bar\theta$, and $U'$, all in the product. Hence $d$ belongs to it, proving $\mathfrak j\bar{\mathfrak j}=(d)$.

The [determinant](../../../../../../determinant.md) of the lattice basis $sd,s(e+\omega)$ gives the [ideal norm](../../../../../../ideal-norm.md) $N(\mathfrak a)=s^2d$. Consequently

$$
\boxed{\mathfrak a\bar{\mathfrak a}=(s^2d)=(N(\mathfrak a))}.
$$

In particular $\langle b,\alpha\rangle\langle b,\bar\alpha\rangle$ is principal. This does not require the original $b$ to be nonzero or the [ideal](../../../../../../ideal.md) itself to be principal.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
