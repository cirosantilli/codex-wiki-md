<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

To distinguish the two normalizations, denote the physicists' [Hermite polynomial](../../../../../../hermite-polynomial.md) by $h_n(x)=(-1)^ne^{x^2}(d/dx)^ne^{-x^2}$. Define the normalized [Hermite functions](../../../../../../hermite-function.md) by

$$
\boxed{H_n(x)=\frac{h_n(x)e^{-x^2/2}}{\pi^{1/4}\sqrt{2^nn!}}.}
$$

Introduce the differential operators $a=(x+d/dx)/\sqrt2$, $a^*=(x-d/dx)/\sqrt2$ on the [Schwartz space](../../../../../../schwartz-space.md). Direct multiplication gives $[a,a^*]=1$ and

$$
-d^2/dx^2+x^2=2a^*a+1.
$$

The Gaussian $H_0=\pi^{-1/4}e^{-x^2/2}$ satisfies $aH_0=0$, and repeated differentiation gives $H_n=(a^*)^nH_0/\sqrt{n!}$. The [commutator](../../../../../../commutator.md) identity implies $aH_n=\sqrt nH_{n-1}$ and $a^*H_n=\sqrt{n+1}H_{n+1}$. Therefore

$$
\boxed{(-d^2/dx^2+x^2)H_n=(2n+1)H_n.}
$$

For normalization, [integration by parts](../../../../../../integration-by-parts.md) makes $a^*$ the [adjoint operator](../../../../../../adjoint-operator.md) of $a$ on these rapidly decreasing functions, so $\|(a^*)^nH_0\|^2=n!\|H_0\|^2=n!$. Distinct [eigenvalues](../../../../../../eigenvalue.md) of the symmetric [quantum harmonic oscillator](../../../../../../quantum-harmonic-oscillator.md) give orthogonality.

The generating identity follows directly from the Rodrigues definition of the [Hermite polynomials](../../../../../../hermite-polynomial.md):

$$
\sum_{n\geq0}\frac{h_n(x)}{n!}w^n
=e^{x^2}\sum_{n\geq0}\frac{(-w)^n}{n!}(d/dx)^ne^{-x^2}
=e^{x^2}e^{-(x-w)^2}=e^{2xw-w^2}.
$$

The Taylor expansion of the entire Gaussian justifies the middle equality for every complex $w$. Substitute $w=z/\sqrt2$ and the [Bargmann-Fock space](../../../../../../bargmann-fock-space.md) basis $e_n(z)=z^n/\sqrt{n!}$ to obtain

$$
\boxed{\sum_{n\geq0}H_n(x)e_n(z)=A_x(z):=\pi^{-1/4}e^{-x^2/2+\sqrt2xz-z^2/2}.}
$$

The convergence is locally uniform in $z$ by the same entire generating series.

For $0<t<1$, $A_x(\sqrt t\,z)$ belongs to the [Bargmann-Fock space](../../../../../../bargmann-fock-space.md): after writing $z=u+iv$, its squared modulus times $e^{-|z|^2}$ has strictly negative quadratic coefficients $-(1+t)u^2-(1-t)v^2$. Taking the [Bargmann-Fock space](../../../../../../bargmann-fock-space.md) inner product of the two generating functions and using the [orthonormal basis](../../../../../../orthonormal-basis.md) proved in part (b) gives

$$
\sum_{n\geq0}t^nH_n(x)H_n(y)
=\frac1\pi\int_{\mathbb C}A_x(\sqrt t\,z)\overline{A_y(\sqrt t\,z)}e^{-|z|^2}\,du\,dv.
$$

The coefficient series converges absolutely by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Substitution factors the right side into

$$
\frac{e^{-(x^2+y^2)/2}}{\pi^{3/2}}
\int_{\mathbb R}e^{-(1+t)u^2+\sqrt{2t}(x+y)u}\,du
\int_{\mathbb R}e^{-(1-t)v^2+i\sqrt{2t}(x-y)v}\,dv.
$$

Use the [Gaussian integral](../../../../../../gaussian-integral.md) $\int e^{-au^2+bu}\,du=\sqrt{\pi/a}\,e^{b^2/(4a)}$ for $a>0$ and complex $b$; the complex case follows from the real case by analyticity. The resulting exponent is

$$
-\frac{x^2+y^2}{2}+\frac{t(x+y)^2}{2(1+t)}-\frac{t(x-y)^2}{2(1-t)}
=\frac{4xyt-(1+t^2)(x^2+y^2)}{2(1-t^2)}.
$$

Thus the [Mehler formula for Hermite functions](../../../../../../mehler-formula-for-hermite-functions.md) is

$$
\boxed{\sum_{n\geq0}t^nH_n(x)H_n(y)=\frac1{\sqrt{\pi(1-t^2)}}\exp\!\left(\frac{4xyt-(1+t^2)(x^2+y^2)}{2(1-t^2)}\right).}
$$

As a normalization check, its $t\downarrow0$ limit is $H_0(x)H_0(y)$. Setting $t=e^{-2s}$ and multiplying by $e^{-s}$ yields the [harmonic oscillator transition kernel](../../../../../../harmonic-oscillator-transition-kernel.md) with [eigenvalues](../../../../../../eigenvalue.md) $2n+1$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
