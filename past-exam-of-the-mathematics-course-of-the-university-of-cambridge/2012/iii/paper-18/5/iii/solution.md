<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

To analyze the [genus one tangent incidence curve of two conics](../../../../../../genus-one-tangent-incidence-curve-of-two-conics.md), choose projective coordinates in which $C_1$ has equation $XZ-Y^2=0$. Its points and tangent lines are parametrized by $[a:b]\in\mathbb P^1$ as

$$
[a^2:ab:b^2],\qquad \ell_{[a:b]}:\ b^2X-2abY+a^2Z=0.
$$

For $x=[X:Y:Z]\in C_2$, the incidence equation is a nonzero homogeneous quadratic in $a,b$, so the projection $E\to C_2$ is finite of degree two. Its discriminant vanishes exactly when $Y^2-XZ=0$, that is, at $C_1\cap C_2$. There are four such points; [Bézout theorem](../../../../../../bezout-s-theorem.md) says their intersection multiplicities sum to four, so all four intersections are transverse.

Locally on $C_2$, after choosing an affine tangent-parameter chart and completing the square, the incidence equation is $w^2=u(s)$, where $s$ is a local parameter and $u$ has a simple zero at each intersection. This is smooth, with ramification index two there; away from those points the roots are distinct and the cover is étale. The analogous chart covers a root at infinity. Thus $E$ is smooth everywhere, and **the cover has exactly four ramification points**. It is connected: the discriminant has odd valuation at each of its four zeros, so it cannot be a square in the function field of $C_2$. The associated quadratic extension is therefore a field, not two separate sheets.

A [smooth plane conic](../../../../../../smooth-plane-conic.md) over $\mathbb C$ is isomorphic to the [projective line](../../../../../../projective-line.md). Apply the [Riemann-Hurwitz formula](../../../../../../riemann-hurwitz-formula.md) to this connected degree-two cover:

$$
2g(E)-2=2(2\cdot0-2)+4=0.
$$

**Consequently $\boxed{g(E)=1}$, and $E$ is a smooth projective [genus one curve](../../../../../../genus-one-curve.md).**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
