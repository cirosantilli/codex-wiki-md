<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The needed [Hensel lemma](../../../../../../hensel-s-lemma.md) says that if $f\in\mathcal O_K[X]$ and $a\in\mathcal O_K$ satisfy $f(a)\equiv0\pmod\pi$ and $f'(a)\not\equiv0\pmod\pi$, then $a$ lifts uniquely to a root of $f$ in $\mathcal O_K$ with the prescribed residue. At every affine point of the smooth curve $\widetilde E$, one partial derivative of its Weierstrass equation is nonzero. Fixing the other coordinate and applying Hensel's lemma lifts that point to $E(K)$; $O_E$ lifts itself. Thus reduction is surjective.

Use the local parameters

$$
t=-x/y,
\qquad z=-1/y,
$$

so $x=t/z$ and $y=-1/z$. Substitution in a general integral Weierstrass equation gives

$$
z=t^3+a_1tz+a_2t^2z+a_3z^2+a_4tz^2+a_6z^3.
$$

For fixed $0\ne t\in\pi\mathcal O_K$, the difference between the two sides, viewed as a polynomial in $z$, is congruent to $z$ modulo $\pi$ and has derivative congruent to one. Hensel's lemma gives a unique $z\in\pi\mathcal O_K$, and therefore a unique point $\theta(t)=(t/z,-1/z)$ in the [kernel of reduction of an elliptic curve](../../../../../../kernel-of-reduction-of-an-elliptic-curve.md). Together with $\theta(0)=O_E$, this identifies that kernel with the parameters $t\in\pi\mathcal O_K$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
