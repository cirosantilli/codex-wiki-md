<h1 id="19/solution">Solution</h1>

↑ **Parent:** [19](../19.md)

For a short string element of length $\Delta x$, the small-slope approximation makes the upward components of [tension](../../../../tension.md) at its two ends $T y_x(x+\Delta x,t)$ and $-Ty_x(x,t)$. Its [mass](../../../../mass.md) is $\rho\Delta x$. [Newton's second law](../../../../newton-s-second-law.md) gives

$$
\rho\Delta x\,y_{tt}=T\left[y_x(x+\Delta x,t)-y_x(x,t)\right].
$$

Divide by $\Delta x$ and take the limit to obtain the [wave equation on a string](../../../../wave-equation-on-a-string.md),

$$
\boxed{y_{tt}=c^2y_{xx},\qquad c=\sqrt{\frac T\rho}}.
$$

Here $\rho$ is [linear mass density](../../../../linear-mass-density.md), and the derivation assumes small transverse slopes, uniform [tension](../../../../tension.md), and a flexible string.

At the right endpoint the string pulls the ring toward the interior. Its vertical force is therefore $-Ty_x(L,t)$ to first order; the frictionless wire supplies no vertical force. The ring obeys

$$
\boxed{M y_{tt}(L,t)=-Ty_x(L,t)}.
$$

This is the dynamic endpoint law for a [string with an endpoint mass](../../../../string-with-an-endpoint-mass.md).

For a separated oscillatory solution, write $y=X(x)q(t)$ with $q''=-\omega^2q$ and $X''+(\omega/c)^2X=0$. The fixed left end removes the spatial [cosine](../../../../cosine.md), so the nonzero [normal modes](../../../../normal-mode.md) have

$$
y_n(x,t)=\left[A_n\cos(\omega_nt)+B_n\sin(\omega_nt)\right]
\sin\frac{\omega_nx}{c}.
$$

The endpoint law gives $M\omega_n^2\sin(\omega_nL/c)=T(\omega_n/c)\cos(\omega_nL/c)$. Since $\sin(\omega_nL/c)=0$ would also force the [cosine](../../../../cosine.md) to vanish, it can be divided out for a nonzero [mode](../../../../mode-statistics.md). Using $T=\rho c^2$ gives

$$
\boxed{\cot\frac{\omega_nL}{c}=\frac{M\omega_n}{\rho c}}.
$$

For physical $M\geq0$, these give all positive modal frequencies. There is no nonzero static linear [mode](../../../../mode-statistics.md): the left value and right slope conditions would force it to vanish. Positivity also follows by [integration by parts](../../../../integration-by-parts.md) from

$$
\omega^2\left(\rho\int_0^L X^2\,dx+MX(L)^2\right)
=T\int_0^L(X')^2\,dx.
$$

For $M=0$, the right endpoint is free, with the [Neumann boundary condition](../../../../neumann-boundary-condition.md) $y_x(L,t)=0$. At $L=\pi$, the allowed wave numbers are $k_n=n+1/2$, $n\geq0$, and $\omega_n=ck_n$. Zero initial displacement removes every cosine-in-time coefficient. The initial velocity contains only the modes $k=1/2$ and $k=5/2$, each with coefficient one. Dividing those velocity coefficients by their angular frequencies gives

$$
\boxed{y(x,t)=\frac2c\sin\frac{ct}{2}\sin\frac x2
+\frac{2}{5c}\sin\frac{5ct}{2}\sin\frac{5x}{2}}.
$$

At $x=0$ each term vanishes, at $x=\pi$ each spatial [derivative](../../../../derivative.md) vanishes, and at $t=0$ the displacement and its time [derivative](../../../../derivative.md) reproduce the two [initial conditions](../../../../initial-condition.md).

## ↑ Ancestors (12)

1. [19](../19.md)
2. [Paper 2](../../paper-2-split.md)
3. [2014](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
