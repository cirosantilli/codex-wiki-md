<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The force from one location is defined [almost surely](../../../../../../almost-sure-convergence.md), since the [uniform distribution](../../../../../../continuous-uniform-distribution.md) assigns probability zero to the origin. Symmetry of that [uniform distribution](../../../../../../continuous-uniform-distribution.md) makes its [characteristic function](../../../../../../characteristic-function.md) real:

$$
q_n(t)=\mathbb E\exp\!\left(\frac{itm\operatorname{sign}(X_1)}{X_1^2}\right)
=\frac1n\int_0^n\cos\!\left(\frac{mt}{x^2}\right)\,dx
=1-\frac{I_n(t)}n,
\qquad I_n(t)=\int_0^n\left(1-\cos\!\left(\frac{mt}{x^2}\right)\right)\,dx.
$$

Near zero the integrand is bounded by $2$. For large $x$ it is at most $m^2t^2/(2x^4)$. The [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) therefore gives the finite [integral](../../../../../../integral.md)

$$
I_n(t)\longrightarrow I(t)=\int_0^\infty\left(1-\cos\!\left(\frac{mt}{x^2}\right)\right)\,dx.
$$

[Independence](../../../../../../independent-random-variables.md) of the locations gives the [characteristic function](../../../../../../characteristic-function.md) of the total force as $q_n(t)^n$. For fixed $t$, $I_n(t)$ is bounded, so [Taylor expansion](../../../../../../taylor-expansion.md) of the [logarithm](../../../../../../logarithm.md) gives

$$
n\log\left(1-\frac{I_n(t)}n\right)=-I_n(t)+O(n^{-1})\longrightarrow-I(t).
$$

The [logarithm](../../../../../../logarithm.md) is legitimate for all sufficiently large $n$.

For $t\ne0$, substitute $u=m|t|/x^2$. The [cosine integral for a symmetric stable exponent](../../../../../../cosine-integral-for-a-symmetric-stable-exponent.md), evaluated directly in part (b), gives

$$
I(t)=\frac{\sqrt{m|t|}}2\int_0^\infty\frac{1-\cos u}{u^{3/2}}\,du
=\sqrt{\frac{\pi m}{2}}\,|t|^{1/2}.
$$

At $t=0$ both sides vanish. The limiting [characteristic function](../../../../../../characteristic-function.md) is [continuous](../../../../../../continuous-function.md) at zero, so the [Lévy continuity theorem](../../../../../../levy-continuity-theorem.md) proves [weak convergence of random variables](../../../../../../convergence-in-distribution.md) to the [symmetric stable distribution](../../../../../../symmetric-stable-distribution.md) of index $1/2$ with

$$
\boxed{\phi(t)=\exp\!\left(-\sqrt{\frac{\pi m}{2}}\,|t|^{1/2}\right).}
$$

The coefficient reflects the spatial density $n/(2n)=1/2$. Symmetry was used in the [characteristic function](../../../../../../characteristic-function.md), without assuming that the singular force has a finite [mean](../../../../../../expected-value.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
