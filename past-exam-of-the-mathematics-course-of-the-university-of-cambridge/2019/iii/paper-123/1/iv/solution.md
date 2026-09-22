<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let

$$
F(X)=X^3+25X^2-50X+40.
$$

Over $\mathbb Q_2$, the [Newton polygon](../../../../../../newton-polygon.md) has three length-one segments of slopes $-2,-1,0$. The resulting roots can also be obtained directly from [Hensel lemma](../../../../../../hensel-s-lemma.md). There is one unit root because $F(1)$ is even and $F'(1)$ is odd. For the two remaining roots, put

$$
F(2Y)=4(2Y^3+25Y^2-25Y+10),
$$

whose parenthesized polynomial has a simple root $Y\equiv1\pmod2$, and

$$
F(4Z)=8(8Z^3+50Z^2-25Z+5),
$$

whose parenthesized polynomial has a simple root $Z\equiv1\pmod2$. Thus $F$ splits completely over $\mathbb Q_2$, with roots of valuations $0,1,2$. There are three primes $q$ above $2$, and for each one

$$
\boxed{L_q=\mathbb Q_2,\qquad \pi_q=2,\qquad k_q=\mathbb F_2.}
$$

Over $\mathbb Q_5$, $F$ is an [Eisenstein polynomial](../../../../../../eisenstein-polynomial.md). Hence there is one prime $q$ above $5$, and if $\alpha$ is the chosen root then

$$
\boxed{L_q=\mathbb Q_5(\alpha),\qquad \pi_q=\alpha,\qquad k_q=\mathbb F_5,}
$$

with $e=3$ and $f=1$.

The polynomial is irreducible over $\mathbb Q$ by the [Eisenstein criterion](../../../../../../eisenstein-criterion.md) at $5$. Its [polynomial discriminant](../../../../../../polynomial-discriminant.md) is

$$
\Delta=-4\cdot25\cdot13807,
$$

which is not a [square number](../../../../../../square-number.md), so the [Galois group of an irreducible cubic](../../../../../../galois-group-of-an-irreducible-cubic.md) is

$$
\boxed{\operatorname{Gal}(E/\mathbb Q)\cong S_3.}
$$

At $2$, all three roots already lie in $\mathbb Q_2$, so the local splitting field is trivial and

$$
\boxed{D_2=I_2=1.}
$$

At $5$, the cubic is totally and tamely ramified. The square class of its discriminant is represented by $-13807\equiv3\pmod5$, a nonsquare unit, so the [quadratic resolvent field of a cubic](../../../../../../quadratic-resolvent-field-of-a-cubic.md) is the unramified quadratic extension of $\mathbb Q_5$. The local splitting field therefore has degree six, with

$$
\boxed{D_5\cong S_3,\qquad I_5\cong A_3\cong C_3.}
$$

These calculations are summarized by [local factorization of X3 plus 25X2 minus 50X plus 40](../../../../../../local-factorization-of-x3-plus-25x2-minus-50x-plus-40.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 123](../../../paper-123-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
