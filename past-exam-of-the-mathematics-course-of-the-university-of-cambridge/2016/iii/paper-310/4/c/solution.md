<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Evaluate the field variance in the zero-occupation [Fock vacuum](../../../../../../fock-vacuum.md), $\hat a_{\mathbf k}|0\rangle=0$, with $[\hat a_{\mathbf k},\hat a_{\mathbf k'}^\dagger]=\delta^3(\mathbf k-\mathbf k')$. The [canonical commutation relation](../../../../../../canonical-commutation-relation.md) alone does not specify a quantum state; this vacuum assumption is needed for the requested expression without occupation factors. In the [Heisenberg picture](../../../../../../heisenberg-picture.md), use the position-space [mode expansion of a free field](../../../../../../mode-expansion-of-a-free-field.md)

$$
\hat v(\tau,\mathbf x)=\int\frac{d^3k}{(2\pi)^{3/2}}
\left[v_k(\tau)e^{i\mathbf k\cdot\mathbf x}\hat a_{\mathbf k}
+v_k^*(\tau)e^{-i\mathbf k\cdot\mathbf x}\hat a_{\mathbf k}^\dagger\right].
$$

This is the position-space form of the shorthand oscillator expansion in the question; equivalently its Fourier operator uses the creation operator with opposite wavevector. The [annihilation operators](../../../../../../annihilation-operator.md) give $\langle\hat a_{\mathbf k}\hat a_{\mathbf k'}^\dagger\rangle=\delta^3(\mathbf k-\mathbf k')$, while all other vacuum pairings vanish. The mean field fluctuation is zero, so the two-point function is its [coincident-point vacuum field variance](../../../../../../coincident-point-vacuum-field-variance.md). Assuming spatial isotropy, angular integration gives the **variance per logarithmic wavenumber interval**:

$$
\boxed{\langle\hat v(\tau,0)\hat v^\dagger(\tau,0)\rangle
=\int\frac{d^3k}{(2\pi)^3}|v_k|^2
=\int_0^\infty\frac{dk}{k}\,\Delta_v(k,\tau),
\qquad \Delta_v=\frac{k^3}{2\pi^2}|v_k|^2.}
$$

Here the [dimensionless power spectrum](../../../../../../dimensionless-cosmological-power-spectrum.md) is denoted $\Delta_v$, as in the question, rather than the alternative notation $\Delta_v^2$. A coincident vacuum field product needs smearing or ultraviolet regulation: the unregulated full vacuum variance is generally divergent. With a specified finite wavenumber band, the same expression holds with those integration limits. This does not affect the mode-by-mode [dimensionless power spectrum](../../../../../../dimensionless-cosmological-power-spectrum.md).

For the leading nonzero slower branch, put $x=-k\tau=k/(aH)>0$ and $v_k=c\,x^{1/2-\nu}/\sqrt{2k}$. Since the physical fluctuation is $\delta\chi=v/a$, its [dimensionless power spectrum](../../../../../../dimensionless-cosmological-power-spectrum.md) is

$$
\begin{aligned}
\Delta_{\delta\chi}
&=\frac{k^3}{2\pi^2a^2}|v_k|^2
=|c|^2\frac{k^2}{4\pi^2a^2}x^{1-2\nu}\\
&=\boxed{|c|^2\left(\frac H{2\pi}\right)^2
\left(\frac{k}{aH}\right)^{3-2\nu}.}
\end{aligned}
$$

For a $k$-independent coefficient $c$, this is a blue [spectral tilt](../../../../../../scalar-spectral-index.md), because $3-2\nu>0$ in the specified mass range. At fixed $k$ it decays as $a^{-(3-2\nu)}$, consistently with the field-amplitude decay found above.

To include the other branch explicitly, the general superhorizon expression is

$$
\Delta_{\delta\chi}=\left(\frac H{2\pi}\right)^2x^3
\left|c_-(k)x^{-\nu}+c_+(k)x^\nu\right|^2.
$$

If $c_-\ne0$, it approaches the displayed target spectrum with $c=c_-$. A pure faster classical branch would instead have power proportional to $x^{3+2\nu}$. For a normalized quantum mode, however, the [Wronskian normalization](../../../../../../wronskian-normalization.md) $v_kv_k^{*\prime}-v_k^*v_k^\prime=i$ requires both independent real solutions; its slower coefficient cannot vanish. Thus the target is the leading superhorizon quantum spectrum, while the faster classical solution remains part of the complete mode analysis.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
