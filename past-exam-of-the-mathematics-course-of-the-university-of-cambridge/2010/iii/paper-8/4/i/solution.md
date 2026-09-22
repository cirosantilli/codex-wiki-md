<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Schwarz lemma](../../../../../../schwarz-lemma.md) states that a [holomorphic function](../../../../../../holomorphic-function.md) $f:\mathbb D\to\mathbb D$ with $f(0)=0$ satisfies

$$
\boxed{|f(z)|\le|z|,\qquad |f'(0)|\le1}.
$$

If equality holds in the first inequality at any nonzero point, or in the derivative inequality, then $f(z)=\lambda z$ for a constant $|\lambda|=1$. Conversely those rotations give equality.

To prove it, the function $g(z)=f(z)/z$ extends holomorphically at zero with value $f'(0)$, by the power series of $f$. On $|z|=r<1$, $|g(z)|\le1/r$. The [maximum modulus principle](../../../../../../maximum-modulus-principle.md) gives this same bound inside that circle. For each fixed $z$, let $r\uparrow1$ to conclude $|g(z)|\le1$. This proves both inequalities. Equality in either makes $g$ attain its maximum modulus at an interior point, so the [maximum modulus principle](../../../../../../maximum-modulus-principle.md) makes $g$ a constant of modulus one. This proves the equality cases as well.

For the classification of [automorphisms of the unit disk](../../../../../../automorphism-of-the-unit-disk.md), choose $a\in\mathbb D$ and define

$$
T_a(z)=\frac{z-a}{1-\overline a z}.
$$

Direct expansion gives

$$
1-|T_a(z)|^2=\frac{(1-|a|^2)(1-|z|^2)}{|1-\overline a z|^2}>0,
\qquad T_a^{-1}(w)=\frac{w+a}{1+\overline a w}.
$$

Thus $T_a$ is a [biholomorphism](../../../../../../biholomorphism.md) of the disk and sends $a$ to zero. If $F$ is any [conformal map](../../../../../../conformal-map.md) of the disk onto itself, take $a=F^{-1}(0)$ and put $h=F\circ T_a^{-1}$. Both $h$ and $h^{-1}$ fix zero. The [Schwarz lemma](../../../../../../schwarz-lemma.md) gives $|h(z)|\le|z|$ and, applied to $h^{-1}$ at $h(z)$, $|z|\le|h(z)|$. Equality holds, so $h(z)=e^{i\theta}z$. Consequently all the holomorphic conformal automorphisms are precisely

$$
\boxed{F(z)=e^{i\theta}\frac{z-a}{1-\overline a z},\qquad |a|<1,\quad\theta\in\mathbb R}.
$$

Every displayed map is indeed a conformal automorphism by the verified inverse and a rotation. Here conformal maps have the usual holomorphic, orientation-preserving meaning; if orientation reversal is allowed, their complex conjugates give the antiholomorphic alternatives.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
