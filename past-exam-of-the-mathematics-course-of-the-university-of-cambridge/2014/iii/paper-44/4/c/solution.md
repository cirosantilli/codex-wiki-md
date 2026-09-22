<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [Minkowski metric](../../../../../../minkowski-metric.md), path-integral weight $e^{iS}$ and the [Abelian gauge theory](../../../../../../abelian-gauge-theory.md) transformation $A_\mu\mapsto A_\mu+\partial_\mu\omega$. The gauge functional $F[A]=\partial\cdot A+A^2$ varies as

$$
\delta_\omega F=(\Box+2A^\mu\partial_\mu)\omega.
$$

Thus the [Faddeev-Popov operator](../../../../../../faddeev-popov-operator.md) is $\mathcal M_A=\Box+2A\cdot\partial$. It depends on the gauge field despite the gauge group being Abelian: **the ghosts interact because this gauge condition is nonlinear**.

Choose the [gauge-fixing fermion](../../../../../../gauge-fixing-fermion.md) $\Psi=\int d^4x\,\bar c(F[A]+\xi h/2)$. The [gauge-fixed action](../../../../../../gauge-fixed-action.md) $S=S_{\rm Maxwell}+s\Psi$ is

$$
\boxed{S=\int d^4x\left[-\frac14F_{\mu\nu}F^{\mu\nu}
+h(\partial\cdot A+A^2)+\frac\xi2h^2
-\bar c(\Box+2A\cdot\partial)c\right].}
$$

Here the tensor $F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu$ is distinct from the scalar gauge functional $F[A]$. With $\xi=0$, integrating over $h$ imposes the exact printed constraint. For nonzero $\xi$, eliminating $h=-F[A]/\xi$ instead gives

$$
\mathcal L=-\frac14F_{\mu\nu}F^{\mu\nu}-\frac1{2\xi}(\partial\cdot A+A^2)^2
-\bar c\Box c-2\bar c A^\mu\partial_\mu c.
$$

This version displays the additional gauge-dependent cubic and quartic gauge-field vertices as well as the ghost interaction; the strict condition is its $\xi\to0$ limit.

For the [Fourier transform](../../../../../../fourier-transform.md) convention $c(x)=\int d^4p\,(2\pi)^{-4}e^{-ipx}c(p)$, the quadratic ghost kernel is $p^2$. With the ordering $\langle c(p)\bar c(q)\rangle$,

$$
\boxed{\langle c(p)\bar c(q)\rangle=(2\pi)^4\delta^{(4)}(p+q)\frac{i}{p^2+i0}.}
$$

The term $-2\bar c A^\mu\partial_\mu c$ has Fourier coefficient $2ip_\mu$, where $p$ is the incoming ghost momentum. Multiplication by $i$ in the [Feynman rule](../../../../../../feynman-rule.md) gives

$$
\boxed{V_\mu(\bar c(q),c(p),A(k))=-2p_\mu,\qquad p+q+k=0.}
$$

These signs refer to the displayed action, Fourier convention and ghost ordering. Reversing the ghost/antighost convention changes corresponding signs consistently. A closed [ghost loop](../../../../../../ghost-loop.md) has the additional minus sign from [Grassmann variables](../../../../../../grassmann-variable.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
