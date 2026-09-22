<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**The displayed estimate has two independent defects.** Even for $a(v)=v$, its right side cannot use $f(t)$. At $t=1$, choose nonnegative [smooth functions](../../../../../../smooth-function.md) $\psi,\chi$ with [compact support](../../../../../../compact-support.md) and prescribe $f(1,x,v)=\psi(x)\chi(v)$. This is a legitimate transported solution with $f_{\mathrm{in}}(x,v)=\psi(x+v)\chi(v)$. The proposed inequality would require

$$
\|\psi\|_\infty\|\chi\|_1
\leq C_a\|\psi\|_1\|\chi\|_\infty.
$$

Velocity dilation makes $\|\chi\|_1/\|\chi\|_\infty$ arbitrarily large, while the other factors stay fixed. Thus no universal $C_a$ works with the same-time [mixed Lebesgue norm](../../../../../../mixed-lebesgue-norm.md).

There is a second issue after replacing $f(t)$ by $f_{\mathrm{in}}$: the [Jacobian determinant](../../../../../../jacobian-determinant.md) bounds give a [local diffeomorphism](../../../../../../local-diffeomorphism.md), not necessarily a one-to-one map. Suppose additionally that $a$ is injective. With $y=x-ta(v)$, the [change of variables formula](../../../../../../change-of-variables-formula.md) and $|\det Da|\geq\alpha_1$ give

$$
\begin{aligned}
\int |f_{\mathrm{in}}(x-ta(v),v)|\,dv
&=\frac1{|t|^d}\int_{x-ta(\mathbb R^d)}
\frac{|f_{\mathrm{in}}(y,a^{-1}((x-y)/t))|}
{|\det Da(a^{-1}((x-y)/t))|}\,dy\\
&\leq \frac1{\alpha_1|t|^d}
\int\sup_w|f_{\mathrm{in}}(y,w)|\,dy .
\end{aligned}
$$

Surjectivity is not needed because the domain of integration can be enlarged. **With injectivity, the corrected estimate has $C_a=1/\alpha_1$.** The upper bound $\alpha_2$ is unnecessary.

More generally, [dispersion with a nonlinear velocity map](../../../../../../dispersion-with-a-nonlinear-velocity-map.md) uses the [area formula](../../../../../../area-formula-geometric-measure-theory.md) to sum over inverse branches. Define the [weighted inverse multiplicity](../../../../../../weighted-inverse-multiplicity.md)

$$
m_a(w)=\sum_{v:\,a(v)=w}\frac1{|\det Da(v)|}.
$$

If $\operatorname*{ess\,sup}_w m_a(w)<\infty$, the same argument gives the corrected estimate with $C_a=\|m_a\|_\infty$. At most $N$ inverse branches give $C_a\leq N/\alpha_1$. Thus the missing global assumption concerns multiplicity, not merely local volume distortion.

For a [noninjective map with constant Jacobian determinant](../../../../../../noninjective-map-with-constant-jacobian-determinant.md) giving a counterexample in two dimensions, write $v=(s,r)$ and set

$$
a(s,r)=e^s\bigl(\cos(re^{-2s}),\sin(re^{-2s})\bigr).
$$

The [polar coordinates](../../../../../../polar-coordinates.md) calculation gives $\det Da=e^{2s}e^{-2s}=1$, yet $a(0,2\pi k)=(1,0)$ for every integer $k$. To turn this into a failure of the estimate, take a small open disk $W$ about $(1,0)$ that avoids the origin. For each of $N$ inverse branches over $W$, choose a smooth cutoff $\chi_k(v)=\chi(a(v))$ supported on that branch, where $\chi$ has support strictly inside $W$ and is extended by zero. These velocity supports are disjoint. Set

$$
f_{\mathrm{in}}(x,v)=\psi(x)\sum_{k=1}^N\chi_k(v).
$$

Then $\|f_{\mathrm{in}}\|_{L_x^1L_v^\infty}=\|\psi\|_1\|\chi\|_\infty$, independent of $N$, whereas at a fixed $t>0$ and suitable $x$,

$$
\int f(t,x,v)\,dv
=N\int_W\psi(x-tw)\chi(w)\,dw.
$$

The last [integral](../../../../../../integral.md) is positive and independent of $N$. No finite $C_a$ exists for this fixed $a$, although $\alpha_1=\alpha_2=1$. In one dimension, by contrast, a nonvanishing derivative has a constant sign, so the lower derivative bound makes $a$ a global [diffeomorphism](../../../../../../diffeomorphism.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
