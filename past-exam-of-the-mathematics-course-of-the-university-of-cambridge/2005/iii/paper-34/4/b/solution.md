<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To keep the normalization visible, denote the integral defining the printed constant by $A_d$. Substituting $r=|y|^2/(2s)$ gives, for $y\ne0$,

$$
\int_0^\infty p(s,0,y)\,ds=A_d|y|^{2-d},\qquad
A_d=\frac{\Gamma(d/2-1)}{2\pi^{d/2}}.
$$

This is the [Newtonian potential of the Brownian heat kernel](../../../../../../newtonian-potential-of-the-brownian-heat-kernel.md). The singularity at zero is locally integrable in dimension $d$, since its radial integral behaves like $\int_0^1r^{2-d}r^{d-1}dr=1/2$. All integrands are nonnegative, so [Tonelli's theorem](../../../../../../tonelli-theorem.md) permits both orders of integration.

Integrating in $s$ first gives

$$
I=A_d\int_{\mathbb R^d}p(t,x,y)|y|^{2-d}\,dy.
$$

Integrating in $y$ first uses the [Gaussian heat kernel](../../../../../../gaussian-heat-kernel.md) [convolution](../../../../../../convolution.md). Completing the square in $|y-x|^2/t+|y|^2/s$ gives

$$
\int_{\mathbb R^d}p(t,x,y)p(s,0,y)\,dy
=(2\pi(t+s))^{-d/2}e^{-|x|^2/(2(t+s))}=p(t+s,0,x).
$$

Consequently $I=\int_t^\infty p(r,0,x)dr$, and the actual identity is

$$
\boxed{\int_{\mathbb R^d}p(t,x,y)|y|^{2-d}\,dy
=A_d^{-1}\int_t^\infty p(r,0,x)\,dr.}
$$

The original PDF uses $A_d$ rather than $A_d^{-1}$ as the multiplier while defining its constant to equal $A_d$. That formula is false. For example $A_3=1/(2\pi)$, so the required multiplier in dimension three is $2\pi$. Equivalently, as $t\downarrow0$ at $x\ne0$, the left side tends to $|x|^{2-d}$, whereas the printed right side tends to $A_d^2|x|^{2-d}$. One can retain the printed form only by defining its multiplier as $c_d=A_d^{-1}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
