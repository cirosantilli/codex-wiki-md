<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Interpret perfect conductivity here as the [perfectly conducting thermal boundary condition](../../../../../../perfectly-conducting-thermal-boundary-condition.md) $\theta=0$; impose the stated magnetic verticality separately. Together with the [stress-free boundary condition](../../../../../../stress-free-boundary-condition.md), admissible vertical profiles are

$$
w=W\sin\pi z,\quad\theta=\vartheta\sin\pi z,\quad\mathbf u_h=\mathbf U_h\cos\pi z,\qquad b_z=Z\cos\pi z,\quad\mathbf b_h=\mathbf B_h\sin\pi z,
$$

each multiplied by $e^{i\mathbf k\cdot\mathbf x+\lambda t}$. Solenoidality requires $i\mathbf k\cdot\mathbf U_h=-\pi W$ and $i\mathbf k\cdot\mathbf B_h=\pi Z$. The [resistive induction equation](../../../../../../resistive-induction-equation.md) preserves both profile choices. In particular $\mathbf b_h=0$ at each boundary and $\partial_zb_z=0$ there.

Set $s=k^2+\pi^2$ and $p=\pi^2$. The pressure-projected vertical momentum, thermal and vertical induction equations reduce to

$$
(\lambda/\sigma+s)W=\frac{Rk^2}{s}\vartheta-Q\zeta\pi Z,\qquad (\lambda+s)\vartheta=W,\qquad (\lambda+\zeta s)Z=\pi W.
$$

Their determinant gives the [vertical-field magnetoconvection dispersion relation](../../../../../../vertical-field-magnetoconvection-dispersion-relation.md)

$$
\boxed{(\lambda+\sigma s)(\lambda+s)(\lambda+\zeta s)+\sigma Q\zeta p(\lambda+s)-\frac{\sigma Rk^2}{s}(\lambda+\zeta s)=0.}
$$

It is best kept as a polynomial rather than canceling a factor that might vanish at a special eigenvalue. For $\lambda=0$,

$$
\boxed{R^{(e)}(k)=\frac{s^3+Qps}{k^2}.}
$$

For an oscillatory marginal mode $\lambda=i\omega$ with $\omega\ne0$, write the polynomial as $\lambda^3+a_1\lambda^2+a_2\lambda+a_3$. Its coefficients are

$$
a_1=(\sigma+1+\zeta)s,\quad a_2=(\sigma+\sigma\zeta+\zeta)s^2+\sigma Q\zeta p-\sigma Rk^2/s,\quad a_3=\sigma\zeta s^3+\sigma Q\zeta ps-\sigma R\zeta k^2.
$$

Separating real and imaginary parts gives $a_3=a_1a_2$ and $\omega^2=a_2>0$. Solving yields

$$
\boxed{R^{(o)}(k)=\frac{(\sigma+\zeta)(1+\zeta)}{\sigma}\frac{s^3}{k^2}+\frac{\zeta(\sigma+\zeta)}{1+\sigma}\frac{Qps}{k^2},\qquad \omega^2=\frac{\sigma\zeta(1-\zeta)}{1+\sigma}Qp-\zeta^2s^2.}
$$

Therefore [oscillatory marginality in vertical-field magnetoconvection](../../../../../../oscillatory-marginality-in-vertical-field-magnetoconvection.md) requires

$$
\boxed{0<\zeta<1,\qquad Q>\frac{\zeta(1+\sigma)}{\sigma(1-\zeta)}\frac{(k^2+\pi^2)^2}{\pi^2}.}
$$

The equality has zero frequency and is not an oscillatory marginal mode. For some positive horizontal [wavenumber](../../../../../../wavenumber.md) to satisfy this condition, it is necessary and sufficient that $Q>\zeta(1+\sigma)\pi^2/[\sigma(1-\zeta)]$, although the associated threshold must still be minimized over admissible modes. When $\omega^2>0$, $R^{(o)}<R^{(e)}$ at the same [wavenumber](../../../../../../wavenumber.md); this also follows from $R^{(e)}-R^{(o)}=(\sigma+1+\zeta)s\omega^2/(\sigma\zeta k^2)$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Section III](../../section-iii.md)
4. [Paper 77](../../../paper-77-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
