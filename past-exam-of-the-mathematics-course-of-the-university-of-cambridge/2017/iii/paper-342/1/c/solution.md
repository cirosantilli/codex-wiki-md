<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Reset $t=0$ when gravity is switched off. The subsequent [overdamped relaxation of a clamped--free filament](../../../../../../overdamped-relaxation-of-a-clamped-free-filament.md) obeys $\zeta_\perp h_t=-Bh_{xxxx}$ with the same homogeneous endpoint conditions. Separate a [normal mode](../../../../../../normal-mode.md) as $h=\phi(x/L)e^{-\Gamma t}$. Writing $s=x/L$ gives

$$
\phi''''=\alpha^4\phi,\qquad \Gamma=\frac{B\alpha^4}{\zeta_\perp L^4}.
$$

The two clamp conditions reduce the general hyperbolic/trigonometric solution to

$$
\phi(s)=C[\cosh(\alpha s)-\cos(\alpha s)]
+D[\sinh(\alpha s)-\sin(\alpha s)].
$$

The two free-end conditions have matrix

$$
\begin{pmatrix}\cosh\alpha+\cos\alpha&\sinh\alpha+\sin\alpha\\
\sinh\alpha-\sin\alpha&\cosh\alpha+\cos\alpha\end{pmatrix}
\begin{pmatrix}C\\D\end{pmatrix}=0.
$$

Its [determinant](../../../../../../determinant.md) is $2(1+\cosh\alpha\cos\alpha)$. Hence the [clamped--free bending mode](../../../../../../clamped-free-bending-mode.md) values satisfy

$$
\cos\alpha_n\cosh\alpha_n=-1,\qquad
\alpha_1=1.8751040687\ldots,\quad\alpha_2=4.6940911330\ldots.
$$

There is no zero mode: at zero eigenvalue $\phi$ is cubic, and the four clamp/free conditions force all coefficients to vanish. With the following normalization a mode is

$$
\phi_n(s)=\cosh(\alpha_ns)-\cos(\alpha_ns)
-\eta_n[\sinh(\alpha_ns)-\sin(\alpha_ns)],\qquad
\eta_n=\frac{\cosh\alpha_n+\cos\alpha_n}{\sinh\alpha_n+\sin\alpha_n}.
$$

The fourth-order operator is [self-adjoint](../../../../../../self-adjoint-operator.md) and positive under these endpoint conditions, since $\int f g''''=\int f''g''$. Its orthogonal [eigenfunction expansion](../../../../../../eigenfunction-expansion.md) gives

$$
h(x,t)=\sum_{n\ge1}c_n\phi_n(x/L)
\exp\left[-\frac{B\alpha_n^4t}{\zeta_\perp L^4}\right],\qquad
c_n=\frac{\int_0^Lh(x,0)\phi_n(x/L)dx}{\int_0^L\phi_n(x/L)^2dx}.
$$

For the previously attained steady profile, the first coefficient is nonzero: $h_s$ is positive and the first mode can be chosen positive in the interior. Two applications of [integration by parts](../../../../../../integration-by-parts.md), using both functions' endpoint conditions, also give

$$
c_1=\frac{wL^4}{B\alpha_1^4}
\frac{\int_0^1\phi_1(s)ds}{\int_0^1\phi_1(s)^2ds}.
$$

Thus the dominant long-time answer, including its shape and amplitude, is

$$
\boxed{h(x,t)\sim c_1\phi_1(x/L)e^{-t/\tau_1},\qquad
\tau_1=\frac{\zeta_\perp L^4}{B\alpha_1^4}
=\frac{\zeta_\perp L^4}{12.36236337\ldots\,B}.}
$$

The next mode decays much faster. For other initial shapes with an accidentally zero first-mode projection, the lowest mode with $c_n\ne0$ determines the asymptotic behaviour. The decay time has the correct units and exhibits the strong $L^4$ dependence characteristic of bending opposed by local viscous drag.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
