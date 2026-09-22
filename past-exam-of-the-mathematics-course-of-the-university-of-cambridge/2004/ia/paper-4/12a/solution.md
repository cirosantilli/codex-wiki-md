<h1 id="12a/solution">Solution</h1>

↑ **Parent:** [12A](../12a.md)

The [moment of inertia of a uniform solid cylinder](../../../../../moment-of-inertia-of-a-uniform-solid-cylinder.md) is taken about its symmetry axis. Write its [mass density](../../../../../density.md) as $\rho_c=m/(\pi a^2L)$. A coaxial shell of radius $r$ and thickness $dr$ has [mass](../../../../../mass.md) $dm=2\pi\rho_c Lr\,dr$. Thus

$$
\boxed{I=\int_0^a r^2\,dm=2\pi\rho_c L\int_0^a r^3\,dr
=\frac12ma^2.}
$$

A hollow cylinder would have a different [moment of inertia](../../../../../moment-of-inertia.md); uniform solid density is the intended assumption.

Let $s$ measure the centre's displacement uphill from its initial [position](../../../../../position.md), and choose signed [angular velocity](../../../../../angular-velocity.md) $\omega$ so that uphill [rolling without slipping](../../../../../rolling-without-slipping.md) has $\dot s=a\omega$. Let $F$ be the signed contact [force](../../../../../force.md) uphill. The translation and rotation equations are

$$
m\ddot s=-mg\sin\alpha+F,\qquad I\dot\omega=-aF.
$$

The minus sign in the [torque](../../../../../torque.md) equation follows from the chosen rolling sense: uphill contact [force](../../../../../force.md) opposes the positive spin. Under [rolling without slipping](../../../../../rolling-without-slipping.md), $\ddot s=a\dot\omega$. Eliminating $F$ gives

$$
\left(m+\frac I{a^2}\right)\ddot s=-mg\sin\alpha,
\qquad \ddot s=-\frac23g\sin\alpha,
\qquad F=\frac13mg\sin\alpha.
$$

Using $s(0)=0$ and $\dot s(0)=V$, the no-slip motion and maximum vertical rise are

$$
\boxed{s(t)=Vt-\frac13g\sin\alpha\,t^2,\qquad
h_{\max}=\frac{3V^2}{4g}.}
$$

Indeed the centre turns at $t=3V/(2g\sin\alpha)$, reaching $s_{\max}=3V^2/(4g\sin\alpha)$, whose vertical component is the boxed height. [Conservation of energy](../../../../../conservation-of-energy.md) independently gives the same answer from initial [kinetic energy](../../../../../kinetic-energy.md) $mV^2/2+I(V/a)^2/2=3mV^2/4$.

The available [static friction](../../../../../static-friction.md) is at most $\mu mg\cos\alpha$. It can supply the required uphill [force](../../../../../force.md) exactly when $mg\sin\alpha/3\leq\mu mg\cos\alpha$. Therefore

$$
\boxed{\tan\alpha>3\mu\quad\Longrightarrow\quad\text{slip starts}.}
$$

Interpret the stated friction magnitude as limiting [static friction](../../../../../static-friction.md) and as [kinetic friction](../../../../../kinetic-friction.md) during slip, with the same coefficient. Take $0<\alpha<\pi/2$, $\mu\geq0$. In the slipping regime the contact point moves downhill relative to the slope, so [kinetic friction](../../../../../kinetic-friction.md) acts uphill. To verify this direction rather than assume it unchecked, solve with $F=\mu mg\cos\alpha$. Define $b=g(\sin\alpha-\mu\cos\alpha)>0$. The result is

$$
\boxed{s(t)=Vt-\frac12bt^2,\qquad
v(t)=\dot s=V-bt,\qquad
\omega(t)=\frac Va-\frac{2\mu g\cos\alpha}{a}t.}
$$

The centre's [speed](../../../../../speed.md) is $|V-bt|$, with the sign of $v$ specifying ascent or descent. The contact point's relative [velocity](../../../../../velocity.md) is

$$
w(t)=v(t)-a\omega(t)=-gt(\sin\alpha-3\mu\cos\alpha)<0\qquad(t>0).
$$

Thus the assumed uphill [kinetic friction](../../../../../kinetic-friction.md) is consistent throughout both ascent and descent, including when the centre's [velocity](../../../../../velocity.md) changes sign. There is no later return to [rolling without slipping](../../../../../rolling-without-slipping.md) before reaching the bottom. This is the characteristic [slipping solid cylinder on an incline](../../../../../slipping-solid-cylinder-on-an-incline.md) regime.

The centre turns at $t_*=V/b$, giving

$$
\boxed{h_{\max}=\frac{V^2\sin\alpha}{2g(\sin\alpha-\mu\cos\alpha)}.}
$$

The formulas apply up to the positive return time $t_b=2V/b$. Substitution into the signed [velocity](../../../../../velocity.md) and [angular velocity](../../../../../angular-velocity.md) gives

$$
\boxed{v(t_b)=-V,\qquad\text{speed at return}=V,\qquad
\omega(t_b)=\frac Va\frac{\sin\alpha-5\mu\cos\alpha}{\sin\alpha-\mu\cos\alpha}.}
$$

The return spin can have either sign and vanishes at $\tan\alpha=5\mu$. It reverses when $3\mu<\tan\alpha<5\mu$, although the contact point still slips downhill. The unchanged centre [speed](../../../../../speed.md) does not mean that no [energy](../../../../../energy.md) was dissipated: the rotational [kinetic energy](../../../../../kinetic-energy.md) has decreased. Indeed integrating the frictional power $Fw<0$ gives

$$
K(0)-K(t_b)=\frac{2\mu mV^2\cos\alpha(\sin\alpha-3\mu\cos\alpha)}{(\sin\alpha-\mu\cos\alpha)^2}\geq0,
$$

which agrees with the difference of the initial and final rotational [kinetic energies](../../../../../kinetic-energy.md).

## ↑ Ancestors (10)

1. [12A](../12a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
