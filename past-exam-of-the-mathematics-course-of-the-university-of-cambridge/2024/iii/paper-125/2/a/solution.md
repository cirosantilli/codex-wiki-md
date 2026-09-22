<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Hasse theorem for elliptic curves](../../../../../../hasse-s-theorem-on-elliptic-curves.md) states that, for an elliptic curve over $\mathbb F_q$,

$$
\left|\#E(\mathbb F_q)-(q+1)\right|\leq2\sqrt q.
$$

Let $\pi$ be the [Frobenius isogeny of an elliptic curve](../../../../../../frobenius-isogeny-of-an-elliptic-curve.md) and put $a=q+1-\#E(\mathbb F_q)$. The fixed points of $\pi$ are $E(\mathbb F_q)$, and $1-\pi$ is separable, so

$$
\deg(1-\pi)=\#E(\mathbb F_q).
$$

Hence the [trace of an elliptic-curve endomorphism](../../../../../../trace-of-an-elliptic-curve-endomorphism.md) is

$$
\operatorname{tr}(\pi)=1+\deg\pi-\deg(1-\pi)=a,
$$

while $\deg\pi=q$.

The degree on $\operatorname{End}(E)$ is a nonnegative quadratic form. Polarization and the identities for the [dual isogeny](../../../../../../dual-isogeny.md) give, for integers $m,n$,

$$
\deg([m]+[n]\pi)=m^2+amn+qn^2.
$$

If $a^2>4q$, this real binary quadratic form is indefinite. An open cone on which it is negative contains a nonzero rational point and therefore a nonzero integer point, contradicting nonnegativity of isogeny degree. Thus $a^2\leq4q$, which is exactly the claimed inequality.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
