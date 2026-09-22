<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [degree of an isogeny](../../../../../degree-of-an-isogeny.md) $\phi:E\to E'$ is the degree of the induced finite extension of function fields. Saying that degree is a quadratic form on $\operatorname{End}(E)$ means

$$
\deg(n\phi)=n^2\deg\phi
$$

and that

$$
\langle\phi,\psi\rangle=\frac12\bigl(\deg(\phi+\psi)-\deg\phi-\deg\psi\bigr)
$$

is bilinear, equivalently

$$
\deg(\phi+\psi)+\deg(\phi-\psi)=2\deg\phi+2\deg\psi.
$$

The [trace of an elliptic-curve endomorphism](../../../../../trace-of-an-elliptic-curve-endomorphism.md) is

$$
\operatorname{tr}(\phi)=1+\deg\phi-\deg(1-\phi).
$$

The relation $\phi^2-[\operatorname{tr}\phi]\phi+[\deg\phi]=0$ implies

$$
\operatorname{tr}(\phi^2)=\operatorname{tr}(\phi)^2-2\deg\phi,
$$

the [trace of the square of an elliptic-curve endomorphism](../../../../../trace-of-the-square-of-an-elliptic-curve-endomorphism.md).

The [Hasse theorem for elliptic curves](../../../../../hasse-s-theorem-on-elliptic-curves.md) states that for $E/\mathbb F_q$,

$$
\left|\#E(\mathbb F_q)-(q+1)\right|\leq2\sqrt q.
$$

Let $\pi$ be the [Frobenius isogeny of an elliptic curve](../../../../../frobenius-isogeny-of-an-elliptic-curve.md), put $a=\operatorname{tr}(\pi)$, and note that $\deg\pi=q$ and

$$
\#E(\mathbb F_q)=\deg(1-\pi)=q+1-a.
$$

For integers $m,n$, quadraticity gives

$$
0\leq\deg(m+n\pi)=m^2+amn+qn^2.
$$

This binary quadratic form cannot have positive discriminant, since rational numbers $m/n$ are dense, so $a^2-4q\leq0$. Substitution proves the bound. This is the [degree-form proof of the Hasse bound](../../../../../degree-form-proof-of-the-hasse-bound.md).

Both endpoints occur. The curve $E:y^2=x^3-x$ over $\mathbb F_3$ is supersingular with trace zero. Over $\mathbb F_9$, its Frobenius is $[-3]$, so

$$
\#E(\mathbb F_9)=9+1-(-6)=16=9+1+2\sqrt9.
$$

Its nontrivial [quadratic twist](../../../../../quadratic-twist-of-an-elliptic-curve.md) over $\mathbb F_9$ has the opposite trace and therefore has

$$
9+1-6=4=9+1-2\sqrt9
$$

points.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 125](../../paper-125-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
