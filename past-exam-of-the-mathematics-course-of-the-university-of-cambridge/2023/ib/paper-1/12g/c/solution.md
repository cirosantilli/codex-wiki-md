<h1 id="12g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [residue theorem](../../../../../../residue-theorem.md) states that if a meromorphic [function](../../../../../../function-split.md) has finitely many poles inside a positively oriented simple closed contour and none on it, then its contour [integral](../../../../../../integral.md) is $2\pi i$ times the sum of the enclosed residues.

Apply it to

$$
F(z)=\frac{e^{\alpha L(z)}}{(1+z)^2}
$$

on a keyhole contour around the positive real axis. The outer and inner circles vanish as their radii tend to infinity and zero because $\alpha<1$ and $\alpha>-1$, respectively. On the upper bank the numerator tends to $x^\alpha$, while on the lower bank it tends to $e^{2\pi i\alpha}x^\alpha$ and the direction is reversed. Therefore the limiting contour [integral](../../../../../../integral.md) is

$$
(1-e^{2\pi i\alpha})I.
$$

The only enclosed pole is the double pole at $z=-1$. Since $L(-1)=i\pi$,

$$
\operatorname{Res}_{z=-1}F
=\left.\frac d{dz}e^{\alpha L(z)}\right|_{z=-1}
=-\alpha e^{i\pi\alpha}.
$$

The residue theorem now gives

$$
(1-e^{2\pi i\alpha})I=-2\pi i\alpha e^{i\pi\alpha}.
$$

For $\alpha\ne0$, division and

$$
1-e^{2\pi i\alpha}=-2ie^{i\pi\alpha}\sin(\pi\alpha)
$$

yield

$$
\boxed{I=\frac{\pi\alpha}{\sin(\pi\alpha)}}.
$$

At $\alpha=0$, the [integral](../../../../../../integral.md) is one, agreeing with the continuous [limit](../../../../../../limit-of-a-function.md). This is the [positive-axis keyhole beta integral](../../../../../../positive-axis-keyhole-beta-integral.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12G](../../12g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
