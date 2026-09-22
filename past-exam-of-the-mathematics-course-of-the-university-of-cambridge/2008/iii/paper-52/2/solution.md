<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Start by using the metric equation of the [Polyakov action](../../../../../polyakov-action.md) to retain the [Virasoro constraints](../../../../../virasoro-constraint.md) after choosing [conformal gauge](../../../../../conformal-gauge.md). In the [light-cone gauge in string theory](../../../../../light-cone-gauge-in-string-theory.md), make $X^+$ proportional to [worldsheet](../../../../../worldsheet.md) time on a patch with nonzero $k^+$. The constraints determine $X^-$ from the transverse coordinates, so its oscillators are not independent physical excitations. [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) make each transverse coordinate a cosine standing wave on the open interval. Quantize these waves as independent [harmonic oscillators](../../../../../simple-harmonic-motion.md) and build their [Fock space](../../../../../fock-space.md) on the momentum-labelled vacuum. There are $d-2=24$ transverse directions in the critical bosonic string, and the normal-ordering intercept is one. Thus physical oscillator states have nonnegative occupation numbers $r_{n,i}$ and level $p=\sum_{n,i}n r_{n,i}$, with $M^2=(p-1)/\alpha'$. Continuous center-of-mass momentum is not part of the discrete oscillator degeneracy.

For each mode $n$ and transverse direction, summing its occupation numbers gives $\sum_{r\ge0}w^{nr}=(1-w^n)^{-1}$. Therefore the [open-string oscillator degeneracy](../../../../../open-string-oscillator-degeneracy.md) generating function is

$$
F(w)=\sum_{p\ge0}d_pw^p=\prod_{n\ge1}(1-w^n)^{-24},
\qquad
\boxed{d_p=\frac1{2\pi i}\oint F(w)w^{-p-1}\,dw.}
$$

This is the [Cauchy coefficient formula](../../../../../cauchy-coefficient-formula.md). The original PDF's power $w^{-p}$ is an index error: it extracts $d_{p-1}$, and would give zero for the vacuum $p=0$, which actually has one oscillator state. Any positively oriented circle strictly inside the unit disk works.

Put $w=e^{-t}$ with $t>0$. Expand the logarithm and sum the geometric series to obtain

$$
\log F(e^{-t})=24\sum_{m\ge1}\frac1{m(e^{mt}-1)}.
$$

Since $t/(e^{mt}-1)\le1/m$, dominated convergence gives $t\log F(e^{-t})\to24\sum_{m\ge1}m^{-2}=4\pi^2$. Thus the leading singular term is $4\pi^2/t$.

The subleading term printed in the PDF also needs correction: the product implies $+12\log\epsilon$, rather than $-6\log\epsilon$. To obtain the coefficient needed for the final power law, use $\tau=it/(2\pi)$ and the [Dedekind eta function](../../../../../dedekind-eta-function.md). Its definition gives $F(e^{-t})=e^{-t}\eta(\tau)^{-24}$. The modular identity $\eta(-1/\tau)=\sqrt{-i\tau}\eta(\tau)$, recorded in [NIST's eta transformation formulas](https://dlmf.nist.gov/23.18), and the product at large imaginary argument give

$$
\boxed{F(e^{-t})=\left(\frac{t}{2\pi}\right)^{12}
\exp\left(\frac{4\pi^2}{t}-t\right)
\left[1+O(e^{-4\pi^2/t})\right].}
$$

Since $t=-\log(1-\epsilon)=\epsilon+\epsilon^2/2+O(\epsilon^3)$, this yields

$$
\log F(1-\epsilon)=\frac{4\pi^2}{\epsilon}+12\log\epsilon
-12\log(2\pi)-2\pi^2+O(\epsilon).
$$

The printed logarithmic correction cannot be used to derive the stated $p^{-27/4}$ prefactor; the corrected correction does.

For the [saddle-point approximation](../../../../../saddle-point-approximation.md), change the coefficient contour to $t=-\log w$. Its local contribution is

$$
d_p\simeq\frac1{2\pi i}\int\left(\frac{t}{2\pi}\right)^{12}e^{S(t)}\,dt,
\qquad S(t)=(p-1)t+\frac{4\pi^2}{t}.
$$

Set $q=p-1$. The positive saddle is $t_0=2\pi/\sqrt q$, with $S(t_0)=4\pi\sqrt q$ and $S''(t_0)=q^{3/2}/\pi$. Along the local vertical steepest-descent direction $t=t_0+iy$, the exponent is $S(t_0)-S''(t_0)y^2/2$ to quadratic order. The factor $(t/2\pi)^{12}$ varies negligibly over its Gaussian width. Hence

$$
d_p\sim\frac{(t_0/2\pi)^{12}}{\sqrt{2\pi S''(t_0)}}e^{S(t_0)}
=\frac1{\sqrt2}q^{-27/4}e^{4\pi\sqrt q}
\sim\boxed{\frac1{\sqrt2}p^{-27/4}e^{4\pi\sqrt p}.}
$$

This proves the [large-level degeneracy of an open bosonic string](../../../../../large-level-degeneracy-of-an-open-bosonic-string.md), including the otherwise unspecified leading constant. The factor $p^{-6}$ comes from the eta prefactor and $p^{-3/4}$ from the saddle width. As allowed, no bound on the remote part of the contour is needed.

At high mass, $p\simeq\alpha'M^2$, so the density grows exponentially as $e^{\beta_HM}$ with

$$
\boxed{\beta_H=4\pi\sqrt{\alpha'},\qquad T_H=\frac1{4\pi\sqrt{\alpha'}}}
$$

in units $k_B=\hbar=c=1$. A canonical sum with $e^{-\beta M}$ cannot converge for $\beta<\beta_H$, regardless of polynomial prefactors. This suggests a Hagedorn threshold and a breakdown or transition of the ordinary dilute-string thermal description. The power prefactor can make the partition sum itself finite at the threshold while sufficiently high energy moments diverge; the asymptotic count alone does not prove an absolute upper temperature. These are properties of the formal high-level spectrum, separate from the [tachyon](../../../../../tachyon.md) instability of the bosonic vacuum.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
