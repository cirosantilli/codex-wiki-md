<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At $r=s=0$, the linear growth rate of a [Fourier mode](../../../../../../fourier-mode.md) $e^{ikx}$ is $-(1-k^2)^2$. Its critical [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md) has $k=\pm1$. Write

$$
w_1=A(X,T)e^{ix}+\overline{A(X,T)}e^{-ix}.
$$

For a compatible periodic carrier, the slowly varying envelope is periodic on $0\le X\le\varepsilon^2L$. Small carrier detuning can alternatively be included in the envelope [wave phase](../../../../../../phase-waves.md).

With $w=O(\varepsilon)$, $r=\varepsilon^4\mu$ and $s=\varepsilon^2\hat s$, all three terms $rw$, $sw^3$, $w^5$ first appear at $O(\varepsilon^5)$. Balancing the time [derivative](../../../../../../derivative.md) thus requires $T=\varepsilon^4t$. Since the linear growth rate near $k=1$ is $-4(k-1)^2+O((k-1)^3)$, spatial detuning must be $O(\varepsilon^2)$ to contribute at the same order. Consequently

$$
\boxed{X=\varepsilon^2x,\qquad T=\varepsilon^4t.}
$$

Treating $x,X$ independently, let $D=\partial_x$ on the fast carrier. Expansion of the linear operator gives

$$
(1+(D+\varepsilon^2\partial_X)^2)^2
=(1+D^2)^2+4\varepsilon^2(1+D^2)D\partial_X
+\varepsilon^4(2+6D^2)\partial_X^2+O(\varepsilon^6).
$$

The $O(\varepsilon^3)$ term annihilates $w_1$, since $(1+D^2)w_1=0$. At orders two through four there is no nonresonant forcing, and [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md) corrections can be absorbed into the definition of $A$, allowing $w_2=w_3=w_4=0$. At order five the equation for $w_5$ is

$$
(1+D^2)^2w_5=\mu w_1+\hat s w_1^3-w_1^5+4w_{1,XX}-w_{1,T}.
$$

The fast operator is a [self-adjoint operator](../../../../../../self-adjoint-operator.md) on periodic functions. Its [Fredholm alternative](../../../../../../fredholm-alternative.md) requires the right-hand side to have zero [inner product](../../../../../../inner-product.md) with each [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md) mode $e^{\pm ix}$, equivalently to have zero resonant [Fourier coefficients](../../../../../../fourier-coefficient.md). The coefficient of $e^{ix}$ in $w_1^3$ is $3A^2\overline A$, and in $w_1^5$ it is $\binom53A^3\overline A^2=10A|A|^4$. Therefore the [solvability condition](../../../../../../solvability-condition.md) is

$$
\boxed{A_T=\mu A+3\hat s A|A|^2-10A|A|^4+4A_{XX}.}
$$

The conjugate condition supplies the same real equation for the negative mode. The remaining noncritical harmonics determine $w_5$ without obstruction. This is the [cubic-quintic Swift–Hohenberg amplitude reduction](../../../../../../cubic-quintic-swift-hohenberg-amplitude-reduction.md); it retains quintic saturation because the small positive cubic coefficient makes the onset mildly subcritical.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
