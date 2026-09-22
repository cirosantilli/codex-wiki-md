<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $E:y^2=x^3+1$, let $\alpha(x,y)=(\zeta x,y)$. The three points $P,\alpha P,\alpha^2P$ lie on the horizontal line through $P$, so their sum is zero. Thus

$$
\alpha^2+\alpha+1=0
$$

in the [endomorphism ring of an elliptic curve](../../../../../../endomorphism-ring-of-an-elliptic-curve.md). Since $\deg\alpha=1$ and complex conjugation sends $\alpha$ to $\alpha^2$, degree on $\mathbb Z[\alpha]$ is the [Eisenstein-integer norm](../../../../../../eisenstein-integer-norm.md):

$$
\deg(m+n\alpha)
=(m+n\alpha)(m+n\alpha^2)
=m^2-mn+n^2.
$$

A separable isogeny is determined by its kernel up to unique isomorphism of its target, and every finite Galois-stable subgroup of an elliptic curve is the kernel of the corresponding quotient isogeny. Put $T=(-1,0)$. The three nonzero points of $E[2]$ are $T,\alpha T,\alpha^2T$, and

$$
(\alpha-\alpha^2)T=\alpha T+\alpha^2T=T.
$$

Hence $\varphi(\alpha-\alpha^2)$ kills $\ker\varphi=\{O,T\}$ and factors uniquely through $\varphi$:

$$
\varphi(\alpha-\alpha^2)=\psi\varphi
$$

for an isogeny $\psi:E'\to E'$. Degrees give

$$
\deg\psi=\deg(\alpha-\alpha^2)=3.
$$

Moreover,

$$
(\alpha-\alpha^2)^2=\alpha+alpha^2-2=-3.
$$

Composing the factorization twice and using the surjectivity of $\varphi$ gives $\psi^2=[-3]$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
