<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**A bounded-domain hypothesis is needed for the requested global construction and uniqueness.** The printed question does not include it. For example, the upper half-plane satisfies the stated [exterior cone condition](../../../../../../exterior-cone-condition.md), but both $u=0$ and $u(x_1,x_2)=x_2$ are [harmonic functions](../../../../../../harmonic-function.md) with zero [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md). Thus part (iv), in its printed unrestricted solution class, is false. In this question's solutions we add that $\Omega$ is bounded; the [exterior cone condition](../../../../../../exterior-cone-condition.md) and all other data remain as printed.

The half-plane also rules out the printed global separated barrier. In its angular interval $(0,\pi)$, varying $r$ on a fixed ray forces $\nu=2$ if $r^{\nu-2}(h''+\nu^2h)\geq\delta>0$ for every $r>0$. We would then have $h''+4h\geq\delta$ and $h<0$. Put $a=\pi/4$ and $b=3\pi/4$. Twice [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\int_a^b(h''+4h)\sin(2(\theta-a))\,d\theta=2\bigl(h(a)+h(b)\bigr)<0,
$$

contradicting the positive integrand. Thus a source qualification is necessary for part (i) as well as part (iv).

Fix $x_0$ and its exterior cone of half-angle $\alpha$. Choose $0<\alpha_0<\min(\alpha,\pi/2)$ and set

$$
\beta=\frac{\pi}{2(\pi-\alpha_0)},\qquad 0<\nu<\beta<1.
$$

On the complement of the cone, unwrap the angle in [polar coordinates](../../../../../../polar-coordinates.md) as $\vartheta\in(\alpha,2\pi-\alpha)$, measured from the cone axis. Then $\psi=\vartheta-\pi$ is the angle from the opposite axis and $|\psi|\leq\pi-\alpha$ on $\overline\Omega\setminus\{x_0\}$. Define the [power barrier for an exterior cone](../../../../../../power-barrier-for-an-exterior-cone.md) by

$$
\boxed{g(r,\vartheta)=-r^\nu\cos\bigl(\beta(\vartheta-\pi)\bigr),\qquad g(x_0)=0.}
$$

This has the requested separated form $r^\nu h(\vartheta)$. In the printed signed-angle convention, the same function is $-r^\nu\cos(\beta(\pi-|\theta|))$ outside the cone. It is smooth across the negative axis: near that axis the angular expression is the even function $\cos(\beta\psi)$.

Since $\beta(\pi-\alpha)<\pi/2$, put $m=\cos(\beta(\pi-\alpha))>0$. The cosine is at least $m$, so $g\leq-mr^\nu<0$ away from $x_0$, and $g$ is [continuous](../../../../../../continuous-function.md) at $x_0$. The [Laplacian in polar coordinates](../../../../../../laplacian-in-polar-coordinates.md) gives

$$
\Delta g=(\beta^2-\nu^2)r^{\nu-2}\cos(\beta\psi).
$$

Let $D=\sup_{x\in\Omega}|x-x_0|<\infty$. Since $\nu<2$, the [barrier for the Dirichlet problem](../../../../../../barrier-for-the-dirichlet-problem.md) satisfies

$$
\boxed{\Delta g\geq\delta:=(\beta^2-\nu^2)mD^{\nu-2}>0.}
$$

Both the uniform lower bound and the later global comparison use boundedness. In particular, $-g$ is positive at every other boundary point, and is bounded away from zero on boundary sets staying a positive distance from $x_0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
