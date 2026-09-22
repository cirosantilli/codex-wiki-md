<h1 id="b/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\omega$ for the nonzero forcing [frequency](../../../../../frequency.md), to distinguish it from the vertical [velocity](../../../../../velocity.md) $w$. Put $k_z=\pi/h$ and $Z(z)=\cos(\pi(2z+h)/(2h))=-\sin(k_zz)$. Then $Z(0)=Z(h)=0$ and $Z''=-k_z^2Z$, so it meets the rigid-wall conditions. Substituting $w=\operatorname{Re}(f(x)e^{-i\omega t}Z(z))$ into the scalar [wave](../../../../../wave-split.md) equation gives

$$
-\omega^2(f''-k_z^2f)-4\Omega^2k_z^2f=0,
$$

or

$$
\boxed{f''+k_z^2\left(\frac{4\Omega^2}{\omega^2}-1\right)f=0,\qquad f(0)=a.}
$$

The [radiation sign for an inertial wave](../../../../../radiation-sign-for-an-inertial-wave.md) must exclude any disturbance arriving from $x=+\infty$. This means an [radiation condition](../../../../../radiation-condition.md) for propagating [waves](../../../../../wave-split.md), or bounded decay for an evanescent [wave](../../../../../wave-split.md).

For $0<|\omega|<2|\Omega|$, put $q=k_z\sqrt{4\Omega^2/\omega^2-1}$. The solutions are oscillatory. The [inertial-wave dispersion relation](../../../../../inertial-wave-dispersion-relation.md) is $\omega^2=4\Omega^2k_z^2/(k_x^2+k_z^2)$; its horizontal [group velocity](../../../../../group-velocity.md) is $c_{g,x}=-\omega k_x/(k_x^2+k_z^2)$. Positive energy transport into the channel therefore requires $k_x=-\operatorname{sgn}(\omega)q$. The solution is

$$
\boxed{w(x,z,t)=\operatorname{Re}\left[a\,e^{-i\operatorname{sgn}(\omega)qx-i\omega t}\cos\left(\frac\pi{2h}(2z+h)\right)\right].}
$$

For a positive [frequency](../../../../../frequency.md), the phase travels towards negative $x$ while the [group velocity](../../../../../group-velocity.md) travels towards positive $x$. Choosing the outgoing sign from the [phase velocity](../../../../../phase-velocity.md) alone would give the wrong result.

For $|\omega|>2|\Omega|$, set $\kappa=k_z\sqrt{1-4\Omega^2/\omega^2}$. Excluding the exponentially growing solution gives

$$
\boxed{w(x,z,t)=\operatorname{Re}\left[a\,e^{-\kappa x-i\omega t}\cos\left(\frac\pi{2h}(2z+h)\right)\right].}
$$

This disturbance decays away from the wavemaker and does not propagate horizontally. At the cutoff the ODE degenerates to $f''=0$; zero [frequency](../../../../../frequency.md) is not a nonzero forced harmonic mode with this vertical shape.

There is a second printed inconsistency: the stated [velocity](../../../../../velocity.md) $u\mathbf i+w\mathbf k$, if taken literally with no $y$ dependence and no transverse [velocity](../../../../../velocity.md), cannot support a nontrivial rotating [inertial wave](../../../../../inertial-wave.md). Its transverse [momentum](../../../../../momentum-split.md) equation would give $2\Omega u=0$, then continuity and the rigid walls would [force](../../../../../force-split.md) $w=0$. The scalar solutions above are the intended inertial-[wave](../../../../../wave-split.md) solutions when two-dimensional means dependence on $x,z$ while **retaining the transverse component $v$**. For a mode, $-i\omega v+2\Omega u=0$ explicitly supplies the generally nonzero transverse [velocity](../../../../../velocity.md). Thus the scalar equation can be solved as requested, but the full [vector](../../../../../vector.md) field needs this correction to the printed two-component description.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
