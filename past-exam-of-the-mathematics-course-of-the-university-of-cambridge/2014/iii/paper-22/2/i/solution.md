<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\pi$ denote the [Frobenius isogeny of an elliptic curve](../../../../../../frobenius-isogeny-of-an-elliptic-curve.md) and write $N=\#E(\mathbb F_q)$. Its [degree of an isogeny](../../../../../../degree-of-an-isogeny.md) is $q$. The [isogeny of elliptic curves](../../../../../../isogeny-of-elliptic-curves.md) $1-\pi$ has differential equal to the identity because $d\pi=0$, so it is a [separable isogeny](../../../../../../separable-isogeny.md). Its kernel consists precisely of the [rational points](../../../../../../rational-point.md) fixed by $\pi$, giving

$$
\deg(1-\pi)=N.
$$

We use the [degree parallelogram law](../../../../../../divisor-proof-of-the-degree-parallelogram-law.md) for [isogenies of elliptic curves](../../../../../../isogeny-of-elliptic-curves.md), with degree zero assigned to the zero map:

$$
\deg(f+g)+\deg(f-g)=2\deg f+2\deg g,\qquad \deg[n]=n^2.
$$

One explanation of the first identity is the [divisor proof of the degree parallelogram law](../../../../../../divisor-proof-of-the-degree-parallelogram-law.md): on $E\times E$, the zero [divisor](../../../../../../divisor.md) of $x(P)-x(Q)$ is the sum of the diagonal and the graph of negation, while its pole [divisor](../../../../../../divisor.md) is twice each coordinate copy of $O$. Pulling the associated [line bundle](../../../../../../line-bundle.md) identity back by $(f,g)$ and taking degrees gives the identity, including exceptional cases by the line-bundle formulation. This works for a general [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md), including characteristic two; $x$ is the quotient coordinate for negation. Polarization therefore makes degree a [quadratic form](../../../../../../quadratic-form.md) on the [endomorphism ring of an elliptic curve](../../../../../../endomorphism-ring-of-an-elliptic-curve.md).

Set $a=q+1-N$, the [Trace of Frobenius](../../../../../../trace-of-frobenius.md). The cross term is determined by $\deg(1-\pi)=1+q-a$, giving, for all integers $m,n$,

$$
\deg([m]-[n]\pi)=m^2-amn+qn^2\geq0.
$$

If $a^2>4q$, the real degree-two [polynomial](../../../../../../polynomial-split.md) $X^2-aX+q$ is negative on a nonempty open interval. That interval contains a rational $m/n$, contradicting the displayed nonnegativity after multiplication by $n^2$. Thus $a^2\leq4q$. **Hasse's bounds are**

$$
\boxed{q+1-2\sqrt q\ \leq\#E(\mathbb F_q)\ \leq q+1+2\sqrt q.}
$$

The argument proves the [Hasse theorem for elliptic curves](../../../../../../hasse-s-theorem-on-elliptic-curves.md) without assuming its bound in advance.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
