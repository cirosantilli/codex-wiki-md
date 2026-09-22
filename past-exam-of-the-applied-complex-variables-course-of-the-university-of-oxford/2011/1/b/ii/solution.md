<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Starting from the [hodograph plane](../../../../../hodograph-plane.md), take the [complex power](../../../../../complex-exponentiation.md)

$$
s=q^{4/3},\qquad0<\arg q<3\pi/4.
$$

It takes the [velocity](../../../../../velocity.md) sector bijectively to the upper half of the [unit disk](../../../../../unit-disk.md). The [boundary](../../../../../boundary-of-a-set.md) points representing the upstream end, the corner and the downstream end become $-1$, zero and one. Next use the [Möbius transformation](../../../../../mobius-transformation.md)

$$
T=\frac{s+1}{s-1}.
$$

The diameter $-1<s<1$ maps to the negative real axis, while for $s=e^{i\theta}$ on the upper semicircle,

$$
T=-i\cot(\theta/2),
$$

which is on the negative imaginary axis. The interior maps to the third quadrant. Squaring therefore gives a [conformal](../../../../../conformal-map.md) bijection from that quadrant to the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md):

$$
\eta=T^2=\left(\frac{q^{4/3}+1}{q^{4/3}-1}\right)^2.
$$

The upstream end, corner and downstream end map to zero, one and [infinity](../../../../../infinity.md), respectively. The two walls map to the positive real axis, and the free [boundary](../../../../../boundary-of-a-set.md) maps to the negative real axis.

Independently, the [exponential function](../../../../../exponential-function.md) $\eta=e^{\pi w}$ takes the potential strip to the same [upper half-plane](../../../../../upper-half-plane-complex-analysis.md) with the same [boundary](../../../../../boundary-of-a-set.md) correspondence. The strip height fixes the coefficient $\pi$, and the normalization $w(B)=0$ fixes the remaining positive multiplicative constant in $\eta$ to one. Consequently

$$
\boxed{e^{\pi w}=\left(\frac{(w')^{4/3}+1}{(w')^{4/3}-1}\right)^2.}
$$

One can make the branches explicit. In the strip, $p=e^{\pi w/2}$ lies in the first quadrant, whereas $T=-p$. Thus

$$
q^{4/3}=\frac{p-1}{p+1}=\tanh\left(\frac{\pi w}{4}\right),\qquad
q=\left[\tanh\left(\frac{\pi w}{4}\right)\right]^{3/4},
$$

with the power taking [arguments](../../../../../argument-complex-analysis.md) in $(0,\pi)$ to $(0,3\pi/4)$. It gives $q\to e^{3\pi i/4}$ upstream, $q\to1$ downstream, and $q\to0$ at $B$, verifying both the branch choice and the [velocity](../../../../../velocity.md) normalization.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the applied complex variables course of the University of Oxford](../../../../split.md)
6. [Applied complex variables course of the University of Oxford](../../../../../applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
