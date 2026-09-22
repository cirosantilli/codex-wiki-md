<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $N=\#E(\mathbb F_q)$. The [Hasse bound](../../../../../../hasse-s-theorem-on-elliptic-curves.md) is

$$
\boxed{|N-(q+1)|\leq2\sqrt q.}
$$

We prove it using [isogeny degrees](../../../../../../degree-of-an-isogeny.md) of [endomorphisms](../../../../../../endomorphism.md), with no assumption about a pre-existing Frobenius eigenvalue estimate. The standard [elliptic isogeny](../../../../../../isogeny-of-elliptic-curves.md) facts we use are these: [isogeny degree](../../../../../../degree-of-an-isogeny.md) is multiplicative under composition; $\deg[m]=m^2$; assigning [isogeny degree](../../../../../../degree-of-an-isogeny.md) zero to the zero [homomorphism](../../../../../../homomorphism.md) makes [isogeny degree](../../../../../../degree-of-an-isogeny.md) a [quadratic form](../../../../../../quadratic-form.md), satisfying the [degree parallelogram law](../../../../../../divisor-proof-of-the-degree-parallelogram-law.md); and the [isogeny degree](../../../../../../degree-of-an-isogeny.md) of a [separable isogeny](../../../../../../separable-isogeny.md) equals the number of its geometric [kernel of an isogeny](../../../../../../kernel-of-an-isogeny.md) points.

Let $\phi$ be the $q$-power [Frobenius isogeny](../../../../../../frobenius-isogeny-of-an-elliptic-curve.md). It has [isogeny degree](../../../../../../degree-of-an-isogeny.md) $q$ and zero differential. Therefore $1-\phi$ has differential the identity and is a [separable isogeny](../../../../../../separable-isogeny.md). Its [kernel of an isogeny](../../../../../../kernel-of-an-isogeny.md) consists exactly of the points fixed by Frobenius, including the identity, so

$$
\deg(1-\phi)=N.
$$

Put $t=q+1-N$. Polarization of the [isogeny degree](../../../../../../degree-of-an-isogeny.md) [quadratic form](../../../../../../quadratic-form.md) gives, for all [integers](../../../../../../integer.md) $m,n$,

$$
\deg([m]-[n]\phi)=m^2-tmn+qn^2.
$$

The cross coefficient is fixed by the case $m=n=1$, where the [isogeny degree](../../../../../../degree-of-an-isogeny.md) is $N=1-t+q$; the coefficients of $m^2,n^2$ are $\deg1=1$ and $\deg\phi=q$.

Every [isogeny degree](../../../../../../degree-of-an-isogeny.md) is nonnegative. For $n\ne0$, divide by $n^2$ to obtain $u^2-tu+q\geq0$ for every rational $u=m/n$. Continuity and density of the rationals imply the same inequality for real $u$. Its minimum, attained at $u=t/2$, is $q-t^2/4$, so $t^2\leq4q$. This is precisely the stated bound. Equality is allowed; a zero value of the [quadratic form](../../../../../../quadratic-form.md) can occur when the two [endomorphisms](../../../../../../endomorphism.md) involved are rationally dependent.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
