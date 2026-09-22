<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\pi$ be the [Frobenius isogeny of an elliptic curve](../../../../../../frobenius-isogeny-of-an-elliptic-curve.md) and put

$$
a=p+1-\#E(\mathbb F_p).
$$

Part (a) gives

$$
\pi^2-[a]\pi+[p]=0.
$$

Let $\alpha,\beta$ be the two roots of $T^2-aT+p$. The points over $\mathbb F_{p^r}$ are exactly $\ker(1-\pi^r)$. Since the differential of $1-\pi^r$ is the identity, this isogeny is separable, and therefore

$$
\#E(\mathbb F_{p^r})=\deg(1-\pi^r).
$$

Using $\deg\psi=(1-\psi)(1-\widehat\psi)$ in the endomorphism algebra gives the [elliptic-curve point count over a finite field](../../../../../../elliptic-curve-point-count-over-a-finite-field.md)

$$
\#E(\mathbb F_{p^r})
=p^r+1-\alpha^r-\beta^r.
$$

Equivalently, if $a_r=\alpha^r+\beta^r$, then

$$
a_0=2,qquad a_1=a,qquad a_r=aa_{r-1}-pa_{r-2},
$$

and $\#E(\mathbb F_{p^r})=p^r+1-a_r$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
