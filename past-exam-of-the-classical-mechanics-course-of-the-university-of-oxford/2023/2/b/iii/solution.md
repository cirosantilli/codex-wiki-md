<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $J=I_1=I_2$, $\omega_3=c$ and

$$
z(t)=\omega_1(t)+i\omega_2(t),\qquad
\nu=\frac{(I_3-J)c}{J}.
$$

Here $c$ and $\nu$ are constant. The first two of [Euler's equations](../../../../../euler-s-equations-rigid-body-dynamics.md) give $\dot\omega_1=-\nu\omega_2+\tau_0/J$ and $\dot\omega_2=\nu\omega_1+\tau_0/J$. Combining them produces

$$
\boxed{\dot z=i\nu z+\frac{\tau_0}{J}(1+i).}
$$

Multiplication by the [integrating factor](../../../../../integrating-factor.md) $e^{-i\nu t}$ gives, for $\nu\ne0$,

$$
z(t)=z(0)e^{i\nu t}+\frac{\tau_0(1+i)}{i\nu J}\left(e^{i\nu t}-1\right).
$$

For completeness, $\nu=0$ instead gives $z(t)=z(0)+\tau_0(1+i)t/J$. These formulas describe a [symmetric top under constant transverse body torque](../../../../../symmetric-top-under-constant-transverse-body-torque.md).

The stated [initial conditions](../../../../../initial-condition.md) require $b\ne0$ and $I_3\ne J$. They give $c=b/(I_3-J)$, $\nu=b/J$ and $z(0)=i\tau_0/b$. Substitution and simplification yield

$$
z(t)=\frac{\tau_0}{b}\left(e^{ibt/J}-1+i\right).
$$

Taking the [real part](../../../../../real-part.md) and [imaginary part](../../../../../imaginary-part.md), the [angular velocity](../../../../../angular-velocity.md) in the [principal body frame](../../../../../principal-body-frame.md) is

$$
\boxed{\boldsymbol\omega(t)=\left(
\frac{\tau_0}{b}\left[\cos\left(\frac{bt}{I_1}\right)-1\right],\quad
\frac{\tau_0}{b}\left[\sin\left(\frac{bt}{I_1}\right)+1\right],\quad
\frac{b}{I_3-I_1}\right).}
$$

Its value at $t=0$ is the required [initial condition](../../../../../initial-condition.md); differentiating the first two components verifies both forced [Euler's equations](../../../../../euler-s-equations-rigid-body-dynamics.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the classical mechanics course of the University of Oxford](../../../../split.md)
6. [Classical mechanics course of the University of Oxford](../../../../../classical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
