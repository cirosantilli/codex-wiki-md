<h1 id="7/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the [thin spherical charge layer limit](../../../../../../../thin-spherical-charge-layer-limit.md), smoothness of $h$ gives

$$
\frac{h(1+\delta)-h(1)}\delta\longrightarrow h'(1).
$$

Thus the shell's total [electric charge](../../../../../../../electric-charge-split.md) tends to $4\pi\rho_0a^3h'(1)$ while its thickness tends to zero. At each fixed $r>a$, the observation point eventually lies outside the shell, whereas at each fixed $r<a$ the interior [electric field](../../../../../../../electric-field-split.md) is unchanged. The limiting [electric field](../../../../../../../electric-field-split.md) away from the [sphere](../../../../../../../sphere.md) is therefore

$$
\mathbf E_0(\mathbf r)=\begin{cases}
\dfrac{\rho_0}{3\epsilon_0}\mathbf r,&r<a,\\
\dfrac{\rho_0a^3}{\epsilon_0r^2}\left[\dfrac13+h'(1)\right]\mathbf e_r,&r>a.
\end{cases}
$$

Its outward-minus-inward jump is

$$
\boxed{\mathbf E_0(a^+)-\mathbf E_0(a^-)=\frac{\rho_0a h'(1)}{\epsilon_0}\mathbf e_r.}
$$

Physically, the limit is a uniformly charged [ball](../../../../../../../ball-mathematics.md) of [charge density](../../../../../../../charge-density.md) $\rho_0$, together with an infinitesimally thin [spherical shell](../../../../../../../spherical-shell.md) of uniform [surface charge density](../../../../../../../surface-charge-density.md)

$$
\boxed{\sigma=\rho_0a h'(1).}
$$

Indeed its [electric charge](../../../../../../../electric-charge-split.md) is $4\pi a^2\sigma$, and the standard normal [electric field](../../../../../../../electric-field-split.md) jump is $\sigma/\epsilon_0$. The [surface charge density](../../../../../../../surface-charge-density.md) can have either sign, or vanish, according to $h'(1)$.

**The order of limits matters.** For every finite $\delta>0$, taking the two one-sided limits at $r=a$ first gives zero jump. The displayed nonzero jump is obtained by first taking $\delta\to0$ at fixed points on either side, then approaching $a$. The value at the [surface](../../../../../../../topological-surface-split.md) itself need not coincide with either trace of the limiting [electric field](../../../../../../../electric-field-split.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
