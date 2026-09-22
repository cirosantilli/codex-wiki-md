<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Hasse theorem for elliptic curves](../../../../../../hasse-s-theorem-on-elliptic-curves.md) states

$$
\boxed{\left|\#E(\mathbb F_q)-(q+1)\right|\le2\sqrt q.}
$$

We prove it by the positive [degree of an isogeny](../../../../../../degree-of-an-isogeny.md). Let $\pi$ be the $q$-power [Frobenius isogeny](../../../../../../frobenius-isogeny-of-an-elliptic-curve.md), of degree $q$. Its fixed points are precisely $E(\mathbb F_q)$, so they form the kernel of $1-\pi$. Since the differential of $\pi$ is zero, the differential of $1-\pi$ is the identity; thus $1-\pi$ is a [separable isogeny](../../../../../../separable-isogeny.md). Its degree is the number of its geometric kernel points. Therefore

$$
N:=\#E(\mathbb F_q)=\deg(1-\pi).
$$

We use the standard [degree parallelogram law](../../../../../../divisor-proof-of-the-degree-parallelogram-law.md), together with $\deg[m]=m^2$: degree, extended by zero at the zero endomorphism, is a positive [quadratic form](../../../../../../quadratic-form.md) on the [endomorphism ring of an elliptic curve](../../../../../../endomorphism-ring-of-an-elliptic-curve.md). Put $t=1+q-N$, the [Trace of Frobenius](../../../../../../trace-of-frobenius.md). Polarizing the degree form gives, for every pair of integers $m,n$,

$$
\deg([m]-[n]\pi)=m^2-tmn+qn^2\ge0.
$$

Indeed, the values on $1$ and $\pi$ are $1$ and $q$, and the cross coefficient is fixed by $\deg(1-\pi)=1+q-t$. These are standard degree facts about [isogenies of elliptic curves](../../../../../../isogeny-of-elliptic-curves.md), which suffice without an assumption about characteristic or ordinariness.

For $n\ne0$, division by $n^2$ shows $x^2-tx+q\ge0$ at every rational $x=m/n$. Density of the [rational numbers](../../../../../../rational-number.md) and continuity of this polynomial make it nonnegative on the real line. Evaluating at its minimum $x=t/2$ gives $q-t^2/4\ge0$, whence $|t|\le2\sqrt q$. Since $N=q+1-t$, this proves the estimate. This is the [degree-form proof of the Hasse bound](../../../../../../degree-form-proof-of-the-hasse-bound.md); it proves both sides simultaneously by positivity of one degree form.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
