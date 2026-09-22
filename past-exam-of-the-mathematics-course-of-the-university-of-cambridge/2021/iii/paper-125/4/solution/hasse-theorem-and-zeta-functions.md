<h1 id="4/solution/hasse-theorem-and-zeta-functions">Hasse theorem and zeta functions</h1>

↑ **Parent:** [Solution](../solution.md)

Let $E$ be an elliptic curve over $\mathbb F_q$ and let $\pi$ be its [Frobenius isogeny](../../../../../../frobenius-isogeny-of-an-elliptic-curve.md). The fixed points of $\pi$ are exactly $E(\mathbb F_q)$, and separability of $1-\pi$ gives

$$
\#E(\mathbb F_q)=\deg(1-\pi)=q+1-a,
$$

Here [Trace of Frobenius](../../../../../../trace-of-frobenius.md) is the integer $a$. Since $\deg\pi=q$, the quadraticity of degree gives, for every pair of integers $m,n$,

$$
0\leq\deg(m-n\pi)=m^2-amn+qn^2.
$$

If the discriminant $a^2-4q$ were positive, this homogeneous quadratic would be negative for some real ratio $m/n$, hence for a nearby rational ratio and then for some pair of integers. Therefore

$$
a^2\leq4q.
$$

This is the [Hasse theorem for elliptic curves](../../../../../../hasse-s-theorem-on-elliptic-curves.md),

$$
\left|\#E(\mathbb F_q)-(q+1)\right|\leq2\sqrt q.
$$

The [Frobenius isogeny](../../../../../../frobenius-isogeny-of-an-elliptic-curve.md) satisfies

$$
\pi^2-a\pi+q=0.
$$

If $\alpha,\beta$ are the roots of $X^2-aX+q$, then $|\alpha|=|\beta|=\sqrt q$ and

$$
\#E(\mathbb F_{q^n})=q^n+1-\alpha^n-\beta^n.
$$

The [zeta function of an elliptic curve over a finite field](../../../../../../zeta-function-of-an-elliptic-curve-over-a-finite-field.md) is

$$
Z(E/\mathbb F_q,T)
=\exp\left(\sum_{n\geq1}\#E(\mathbb F_{q^n})\frac{T^n}{n}\right).
$$

Substitution of the point-count formula and $-\log(1-z)=\sum_{n\geq1}z^n/n$ gives the rational function

$$
Z(E/\mathbb F_q,T)
=\frac{(1-\alpha T)(1-\beta T)}{(1-T)(1-qT)}
=\frac{1-aT+qT^2}{(1-T)(1-qT)}.
$$

The bounds $|\alpha|=|\beta|=\sqrt q$ are the [Riemann hypothesis for an elliptic curve over a finite field](../../../../../../riemann-hypothesis-for-an-elliptic-curve-over-a-finite-field.md). The relations $\alpha\beta=q$ and the displayed formula also give the functional equation

$$
Z(E/\mathbb F_q,1/(qT))=Z(E/\mathbb F_q,T).
$$

## ↑ Ancestors (11)

1. [Solution](../solution.md)
2. [4](../../4.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
