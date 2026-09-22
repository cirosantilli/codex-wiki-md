<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md) and put $z=h\lambda$. Every recurrence mode must satisfy

$$
 P_z(\zeta)=\zeta^2-1-z\{a\zeta^2+2(1-a)\zeta+a\}=0.
$$

The [amplification polynomial of a multistep method](../../../../../../amplification-polynomial-of-a-multistep-method.md), rather than just its root near one, determines [absolute stability](../../../../../../linear-stability-domain.md). Put $B=2a-1$ and use the [Cayley transform between the half-plane and disk](../../../../../../cayley-transform-between-the-half-plane-and-disk.md)

$$
\zeta=\frac{1+w}{1-w},\qquad |\zeta|\leq1\ \Longleftrightarrow\ \operatorname{Re}w\leq0.
$$

For $\zeta\ne-1$, the characteristic equation becomes

$$
2w=z(1+Bw^2),\qquad
\operatorname{Re}z=\frac{2\operatorname{Re}w(1+B|w|^2)}{|1+Bw^2|^2}.
$$

If $B>0$, the denominator cannot vanish at a root of the characteristic equation: $1+Bw^2=0$ would force $w=0$, a contradiction. Hence $\operatorname{Re}z<0$ forces $\operatorname{Re}w<0$, so all amplification roots have [modulus](../../../../../../modulus.md) less than one. On the imaginary axis the roots have [modulus](../../../../../../modulus.md) one and are simple: the transformed quadratic has discriminant $4(1-Bz^2)>0$ for imaginary $z$. At $z=0$ they are the two simple roots $\pm1$. Also $\zeta=-1$ cannot be a root when $B>0$ and $z\ne0$, and the leading coefficient $1-az$ cannot vanish in the closed left half-plane.

If $a<1/2$, the root near $-1$ is

$$
\zeta_-(z)=-1+(1-2a)z+O(z^2).
$$

For small negative real $z$ it lies below $-1$, violating [absolute stability](../../../../../../linear-stability-domain.md). The endpoint $a=1/2$ deserves separate treatment:

$$
 P_z(\zeta)=(\zeta+1)\left\{\zeta-1-\frac z2(\zeta+1)\right\}.
$$

One root is always $-1$; the other is the [trapezoidal rule](../../../../../../trapezoidal-rule.md) multiplier $(1+z/2)/(1-z/2)$. They are distinct for every finite $z$ in the left half-plane. Consequently, with [absolute stability](../../../../../../linear-stability-domain.md) understood as the bounded [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md),

$$
\boxed{\text{A-stability holds exactly for }a\geq\tfrac12.}
$$

There is a convention at this reducible endpoint: if [A-stability](../../../../../../a-stability.md) is defined to require every unreduced recurrence mode to decay for $\operatorname{Re}z<0$, the answer is **$a>1/2$**, since the $(-1)^n$ mode persists at $a=1/2$. Canceling the common factor $\zeta+1$ gives the [A-stable](../../../../../../a-stability.md) [trapezoidal rule](../../../../../../trapezoidal-rule.md), but cancellation removes an actual starting-error mode of the original two-step recurrence. The fourth-order member $a=1/3$ is outside either [A-stability](../../../../../../a-stability.md) range.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Section A](../../section-a.md)
4. [Paper 68](../../../paper-68-split.md)
5. [Iii](../../../split.md)
6. [2015](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
