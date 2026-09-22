<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The relevant boundary values are $a=\pi$ and $\sigma=0$, but the original complex [integral](../../../../../../integral.md) defining $g(0)$ requires $\sigma>0$. Substituting zero into it is invalid: its real part has a nonintegrable $dx/(x\log x)$ singularity near zero. Its imaginary part is different, since for positive $\sigma$

$$
F(t,a,\sigma)=\int_0^\infty
\frac{x^{\sigma-1}e^{-tx}}{a^2+\log^2x}\,dx.
$$

This has a finite limit as $\sigma\downarrow0$. On $(0,1)$, $x^{\sigma-1}\le x^{-1}$, whose displayed logarithmic denominator makes the [integral](../../../../../../integral.md) finite; at infinity, a fixed upper bound on $\sigma$ and exponential damping provide an integrable dominator. Thus [dominated convergence](../../../../../../dominated-convergence-theorem.md) gives $N(t)=\lim_{\sigma\downarrow0}F(t,\pi,\sigma)$.

For the asymptotics, take the imaginary-part parameter identity before passing to that limit, with a fixed $0<s<1/2$. Its endpoint factor converges to

$$
h_0(r)=\frac{\sin(\pi r)}\pi\Gamma(r)=\frac1{\Gamma(1-r)}
$$

by the [Gamma reflection formula](../../../../../../gamma-reflection-formula.md). Near zero, $\sin(\pi r)\Gamma(\sigma+r)$ is bounded uniformly for small $\sigma\ge0$, because the sine zero compensates the gamma pole. At $s>0$, the remainder [integral](../../../../../../integral.md) itself remains absolutely convergent at $\sigma=0$ and is $O(t^{-s})$. Consequently

$$
N(t)=\int_0^s e^{-r\log t}\frac{dr}{\Gamma(1-r)}+O(t^{-s}).
$$

The endpoint function is analytic with value one, so [Watson's lemma](../../../../../../watson-s-lemma.md) proves the [logarithmic expansion of Ramanujan's function](../../../../../../logarithmic-expansion-of-ramanujan-s-function.md)

$$
\boxed{N(t)\sim\sum_{n\ge0}\frac{c_n}{(\log t)^{n+1}},
\qquad\frac1{\Gamma(1-z)}=\sum_{n\ge0}c_n\frac{z^n}{n!}}.
$$

In particular, with $\gamma$ [Euler's constant](../../../../../../euler-s-constant.md),

$$
\boxed{N(t)=\frac1{\log t}-\frac\gamma{(\log t)^2}
+\frac{\gamma^2-\pi^2/6}{(\log t)^3}
+O\bigl((\log t)^{-4}\bigr)}.
$$

This use of [imaginary-part regularization at a zero Mellin exponent](../../../../../../imaginary-part-regularization-at-a-zero-mellin-exponent.md) matters: the positive-$\sigma$ coefficient $\beta_0$ in part (b) is always zero, whereas the boundary endpoint function has $h_0(0)=1$. The fixed-positive-parameter expansion is not uniform as $\sigma\downarrow0$, so its coefficients cannot simply be sent to that boundary term by term.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
