<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Hasse theorem for elliptic curves](../../../../../../hasse-s-theorem-on-elliptic-curves.md) states that every [elliptic curve](../../../../../../elliptic-curve.md) $E/\mathbb F_q$ satisfies

$$
\boxed{\left|\#E(\mathbb F_q)-(q+1)\right|\leq2\sqrt q.}
$$

Let $\pi$ be the [Frobenius isogeny](../../../../../../frobenius-isogeny-of-an-elliptic-curve.md) and put $a=\operatorname{tr}(\pi)$. Its fixed points are exactly $E(\mathbb F_q)$, so separability of $1-\pi$ gives

$$
\#E(\mathbb F_q)=\deg(1-\pi)=1+q-a.
$$

The [degree of an isogeny](../../../../../../degree-of-an-isogeny.md) is a nonnegative [quadratic form](../../../../../../quadratic-form.md) on the endomorphism ring, and for all integers $m,n$,

$$
\deg([m]+[n]\pi)=m^2+amn+qn^2\geq0.
$$

If $a^2>4q$, this quadratic polynomial has two real roots and takes a negative value at some rational $m/n$ between them, hence after clearing denominators at some integer pair $(m,n)$. Therefore $a^2\leq4q$, and substituting $a=q+1-\#E(\mathbb F_q)$ proves the bound. This is the [degree-form proof of the Hasse bound](../../../../../../degree-form-proof-of-the-hasse-bound.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
