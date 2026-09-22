<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [strong-collision ion-neutral Alfvén modes](../../../../../../strong-collision-ion-neutral-alfven-modes.md), put $a=k_\parallel v_A$ and assume $0<|a|/\mu\ll1$. Rewrite the cubic as

$$
i\mu(2\omega^2-a^2)+\omega(\omega^2-a^2)=0.
$$

The two slow roots obey $\omega=O(a)$, so the first approximation is $\omega_0^2=a^2/2$. Set $\omega=\omega_0+\delta\omega$ and retain the next order, of size $a^3$:

$$
4i\mu\omega_0\delta\omega+\omega_0(\omega_0^2-a^2)=0,\qquad4i\mu\omega_0\delta\omega-\frac{a^2\omega_0}{2}=0.
$$

Consequently

$$
\boxed{\omega_\pm=\pm\frac{k_\parallel v_A}{\sqrt2}-i\frac{k_\parallel^2v_A^2}{8\mu}+O\left(\frac{|k_\parallel v_A|^3}{\mu^2}\right).}
$$

These are weakly damped [Alfvén waves](../../../../../../alfven-wave.md). Their [phase speed](../../../../../../phase-speed.md) is $v_A/\sqrt2=B_0/\sqrt{4\pi(\rho_i+\rho_n)}$, since [collisions](../../../../../../collision.md) make the neutral mass participate in the oscillation. Their [ambipolar damping](../../../../../../ambipolar-damping.md) rate is $\Gamma_A=a^2/(8\mu)$, with $\Gamma_A/|\operatorname{Re}\omega_\pm|\ll1$.

For the remaining root, at $a=0$ the cubic is $\omega^2(\omega+2i\mu)$, so start from $\omega_{d0}=-2i\mu$. Denote the cubic by $F(\omega,a)$. Its value and derivative at this root are

$$
F(-2i\mu,a)=i\mu a^2,\qquad \left.\partial_\omega F\right|_{a=0,\,\omega=-2i\mu}=-4\mu^2.
$$

The first correction is therefore $\delta\omega_d=ia^2/(4\mu)$, giving

$$
\boxed{\omega_d=-2i\mu+i\frac{k_\parallel^2v_A^2}{4\mu}+O\left(\frac{k_\parallel^4v_A^4}{\mu^3}\right).}
$$

This branch is purely damped. Indeed, the real growth-rate polynomial for $s=-i\omega$ is $s^3+2\mu s^2+a^2s+\mu a^2$, and its simple real root near $-2\mu$ stays real for sufficiently small real $a^2$. It represents rapid decay of ion-neutral relative motion. In the $a\to0$ limit, the other two [frequencies](../../../../../../frequency.md) tend to zero; all three branches are accounted for.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
