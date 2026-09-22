<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the [Poincaré-Lindstedt method](../../../../poincare-lindstedt-method.md) to the truncated system from part (b). Since $y=\dot x$, its scalar equation is

$$
\ddot x+x=\epsilon\left(5\mu\dot x-3x^2\dot x+2x\dot x^2-2\dot x^3\right).
$$

Introduce the stretched time $\tau=\omega t$, with [asymptotic expansions](../../../../asymptotic-expansion-split.md)

$$
\omega=1+\epsilon\omega_1+O(\epsilon^2),\qquad
x(t)=X(\tau)=A\cos\tau+\epsilon X_1(\tau)+O(\epsilon^2).
$$

Primes in this part mean [derivatives](../../../../derivative.md) with respect to $\tau$. At first order,

$$
X_1''+X_1=2\omega_1A\cos\tau-5\mu A\sin\tau
+3A^3\cos^2\tau\sin\tau+2A^3\cos\tau\sin^2\tau+2A^3\sin^3\tau.
$$

The [trigonometric identities](../../../../trigonometric-identity.md)

$$
\cos^2\tau\sin\tau=\frac{\sin\tau+\sin3\tau}{4},\qquad
\cos\tau\sin^2\tau=\frac{\cos\tau-\cos3\tau}{4},\qquad
\sin^3\tau=\frac{3\sin\tau-\sin3\tau}{4}
$$

reduce this to

$$
X_1''+X_1=
\left(2\omega_1A+\frac{A^3}{2}\right)\cos\tau
+\left(-5\mu A+\frac{9A^3}{4}\right)\sin\tau
-\frac{A^3}{2}\cos3\tau+\frac{A^3}{4}\sin3\tau.
$$

A periodic $X_1$ cannot have a [secular term](../../../../secular-term.md), so both fundamental-harmonic [coefficients](../../../../coefficient.md) must vanish. Taking $A>0$ gives

$$
\boxed{A^2=\frac{20\mu}{9},\qquad \omega_1=-\frac{A^2}{4}=-\frac{5\mu}{9}.}
$$

In particular $\mu>0$ is necessary. Once these conditions hold, a bounded particular correction is

$$
X_1=\frac{A^3}{16}\cos3\tau-\frac{A^3}{32}\sin3\tau;
$$

adding fundamental sine and cosine terms adjusts the [phase](../../../../phase-waves.md) and the first correction to the [amplitude](../../../../wave-amplitude.md). Consequently the required leading [periodic orbit](../../../../periodic-orbit.md) is

$$
\boxed{x=A\cos(\omega t)+O(\epsilon),\quad
y=-A\omega\sin(\omega t)+O(\epsilon),\quad
\omega=1-\frac{5\mu\epsilon}{9}+O(\epsilon^2).}
$$

Here $A$ is the leading [amplitude](../../../../wave-amplitude.md), not an assertion that the exact finite-$\epsilon$ [amplitude](../../../../wave-amplitude.md) is independent of $\epsilon$.

To justify existence beyond formal cancellation, the leading radial displacement in a [Poincaré return map](../../../../poincare-map.md) is $2\pi\epsilon B(r)$, where

$$
B(r)=\frac{5\mu}{2}r-\frac98r^3.
$$

At the positive root $A$, $B'(A)=-5\mu\ne0$. The [implicit function theorem](../../../../implicit-function-theorem.md), applied after dividing the displacement by $\epsilon$, continues this root to a [periodic orbit](../../../../periodic-orbit.md) for sufficiently small positive $\epsilon$. Its radial [Floquet multiplier](../../../../floquet-multiplier.md) is $1-10\pi\mu\epsilon+O(\epsilon^2)$, so it is attracting. These statements apply to the truncated system with fixed $\mu>0$; its interpretation as a local approximation to the original three-dimensional system also requires $\mu$ small, so that $A=O(\sqrt\mu)$ stays near the [Hopf bifurcation](../../../../hopf-bifurcation.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the nonlinear systems course of the University of Oxford](../../../split.md)
5. [Nonlinear systems course of the University of Oxford](../../../../nonlinear-systems-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
