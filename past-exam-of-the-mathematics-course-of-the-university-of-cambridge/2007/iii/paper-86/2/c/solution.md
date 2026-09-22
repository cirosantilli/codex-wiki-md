<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Now $h_1=g_1$ and $h_2=g_2$. Define their [Fourier sine transforms](../../../../../../fourier-sine-transform.md)

$$
S_1(p)=\int_0^\infty\sin(ps)g_1(s)ds,\qquad S_2(p)=\int_0^\infty\sin(ps)g_2(s)ds,\qquad B(p)=\sqrt{p^2+4\lambda}.
$$

First make the elimination from the [global relations](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) explicit. Write $H_j(p)=\int_0^\infty e^{-ips}h_j(s)ds$ and $N_j(p)=\int_0^\infty e^{-ips}n_j(s)ds$. For $p>0$, set $\kappa=(p+B)/2$. Apply the relation of part (a) at the two negative real spectral points $k=-\kappa$ and $k=-\lambda/\kappa$. They have the same $b=-B$ and opposite $a=-p,p$. Subtracting cancels the left derivative transform, and gives

$$
\boxed{\int_0^\infty\sin(px)n_2(x)dx=-B(p)S_2(p)+p\int_0^\infty e^{-B(p)y}g_1(y)dy.}
$$

Likewise use $k=-i\kappa,-i\lambda/\kappa$, which have the same $a=-iB$ and opposite $b=-ip,ip$. Their difference gives

$$
\boxed{\int_0^\infty\sin(py)n_1(y)dy=-B(p)S_1(p)+p\int_0^\infty e^{-B(p)x}g_2(x)dx.}
$$

Thus both unknown normal traces have sine transforms determined by the given data. The reciprocal symmetries of the dispersion curve, rather than an arbitrary assumption about an unknown trace, perform the elimination.

Here is a direct way to finish that elimination in the integral representation of part (b). Its full-plane kernel has Fourier representation

$$
\Gamma(X,Y)=\frac1{4\pi}\int_{\mathbb R}\frac{e^{ipX-B(p)|Y|}}{B(p)}dp,
$$

and solves $(-\Delta+4\lambda)\Gamma=\delta$. Form the four-image kernel

$$
\begin{aligned}
G_Q(x,y;\xi,\eta)={}&\Gamma(x-\xi,y-\eta)-\Gamma(x+\xi,y-\eta)\\
&-\Gamma(x-\xi,y+\eta)+\Gamma(x+\xi,y+\eta).
\end{aligned}
$$

For $x,y>0$, the three reflected source points are outside the quadrant. Their boundary integrals against the solution vanish by [Green second identity](../../../../../../green-second-identity.md); spectrally these are superpositions of the same reflected [global relations](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) used above. Thus replacing $\Gamma$ by $G_Q$ in part (b) does not change $q$. But $G_Q$ vanishes on either boundary, so all terms multiplying unknown normal traces disappear. The remaining inward kernel derivatives reconstruct the value:

$$
q(x,y)=\int_0^\infty g_2(\xi)\,\partial_\eta G_Q(x,y;\xi,0)d\xi+\int_0^\infty g_1(\eta)\,\partial_\xi G_Q(x,y;0,\eta)d\eta.
$$

Differentiate the displayed spectral kernel and combine positive and negative $p$. The bottom derivative is $(2/\pi)\int_0^\infty\sin(px)\sin(p\xi)e^{-B(p)y}dp$, and the left derivative is the corresponding expression with $x,y$ interchanged. This derives the [quadrant modified Helmholtz Dirichlet Poisson formula](../../../../../../quadrant-modified-helmholtz-dirichlet-poisson-formula.md), entirely in known data:

$$
\boxed{q(x,y)=\frac2\pi\int_0^\infty\left[\sin(px)e^{-B(p)y}S_2(p)+\sin(py)e^{-B(p)x}S_1(p)\right]dp.}
$$

It is an integral on the same complex dispersion curve. To display the requested complex $k$-plane contours explicitly, let $a=k-\lambda/k$ and $b=k+\lambda/k$ as before. On the real ray above $\sqrt\lambda$, $p=a$, $B=b$ and $dp=b\,dk/k$. On the imaginary ray above $i\sqrt\lambda$, $p=-ib$, $B=-ia$ and $dp=-ia\,dk/k$. Consequently

$$
\boxed{\begin{aligned}
q(x,y)={}&\frac2\pi\int_{\sqrt\lambda}^{\infty} b\sin(ax)e^{-by}S_2(a)\frac{dk}{k}\\
&+\frac2\pi\int_{i\sqrt\lambda}^{i\infty}(-ia)\sin(-iby)e^{iax}S_1(-ib)\frac{dk}{k}.
\end{aligned}}
$$

Both contours are oriented outward, and the sine-transform arguments on them are positive real numbers. No unknown boundary transform remains.

Every integrand solves $q_{xx}+q_{yy}-4\lambda q=0$, because $B^2-p^2=4\lambda$. As $y\downarrow0$ with $x>0$, the first term tends to $g_2(x)$ by [Fourier sine inversion](../../../../../../fourier-sine-inversion.md) and the second tends to zero by exponential convergence; the left trace follows symmetrically. Although the two separate contributions may have different corner limits, their sum is continuous at the corner when $g_1(0)=g_2(0)$. For example, the local constant-data corner contributions are the complementary angular harmonic weights, whose sum is one; the mass term is lower order under corner rescaling. Equivalently, subtract a smooth local lifting with the common corner value and use the zero-trace quadrant [Green function](../../../../../../green-s-function.md) to obtain a continuous remainder. Decay and uniqueness follow from the positive mass and the [weak maximum principle](../../../../../../weak-maximum-principle-for-elliptic-operators.md), or from the positive energy identity for a difference with zero boundary data.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 86](../../../paper-86-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
