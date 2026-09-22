<h1 id="38b/solution">Solution</h1>

↑ **Parent:** [38B](../38b.md)

Take a horizontally polarized shear displacement $u(y)e^{i(kx-\omega t)}$, with $k>0$ and $c=\omega/k$. In the layer put $q=\sqrt{c^2/\bar c_s^2-1}$ and in the half-space put $\gamma=\sqrt{1-c^2/c_s^2}$. The required inequality makes both positive. The shear-wave equations give

$$
u_{layer}=A\cos[kq(y-h)],\qquad u_{half}=Be^{k\gamma y},
$$

where the first form satisfies zero traction at $y=h$ and the second decays as $y\to-\infty$. Displacement and traction continuity at zero give $A\cos(kqh)=B$ and $\bar\mu kqA\sin(kqh)=\mu k\gamma B$. Hence the [Love wave](../../../../../love-wave.md) dispersion relation is

$$
\boxed{\tan(khq)=\frac{\mu\gamma}{\bar\mu q}.}
$$

The left-hand square root uses the layer speed $\bar c_s$, as in the original PDF; the TeX aid incorrectly omits its bar there.

Let $K=kh>0$ and $q_{max}=\sqrt{c_s^2/\bar c_s^2-1}$. The allowed interval is $0<q<q_{max}$, and the right side becomes

$$
\frac\mu{\bar\mu}\frac{\bar c_s}{c_s}\frac{\sqrt{q_{max}^2-q^2}}q,
$$

a positive strictly decreasing function from infinity to zero. On each positive branch of $\tan(Kq)$ beginning at $Kq=m\pi$, the left side is strictly increasing from zero to infinity, or to a positive endpoint value if $q_{max}$ comes first. There is exactly one intersection on that branch whenever $m\pi<Kq_{max}$. The fundamental branch $m=0$ thus supplies a real solution for every positive $kh$.

The second branch exists precisely when $Kq_{max}>\pi$. Thus the [strict cutoff of the second Love-wave mode](../../../../../strict-cutoff-of-the-second-love-wave-mode.md) is

$$
\boxed{(kh)_{cutoff}=\frac\pi{\sqrt{c_s^2/\bar c_s^2-1}},\qquad
\text{two trapped modes iff }kh>(kh)_{cutoff}.}
$$

At equality the second solution would have $c=c_s$, zero half-space decay exponent, and fails the required disturbance decay. Consequently the cutoff is the infimum, rather than an attained smallest value, under the printed strict speed inequality. Also $kh=0$ itself is a limiting case, not a trapped propagating mode; the “any value” assertion is valid for positive $kh$.

## ↑ Ancestors (10)

1. [38B](../38b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
